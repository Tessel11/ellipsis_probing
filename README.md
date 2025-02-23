# Discontinuous probing

The code that goes alongside our ACL Findings 2022 paper:
    ``Discontinuous Constituency and BERT: A Case Study of Dutch".
    
    
```
@inproceedings{kogkalidis2022discontinuous,
  title = "Discontinuous Constituency and BERT: A Case Study of Dutch",
  author = "Konstantinos Kogkalidis and Gijs Wijnholds",
  year = "2022",
  booktitle={Findings of ACL 2022},
  publisher={Association for Computational Linguistics}
}
```
    
   
# Running the code
* Make a clean virtual environment using python 3.9+
* Install dependencies: `pip install -r requirements.txt`
* Extract data into 'synt_nl2i_eval_torch/evaluation_data'
* Run the code:
```
    from synt_n2li_eval_torch.evaluation.main import do_everything, bertje_name, robbert_name
    results = do_everything('./synt_nl2i_eval_torch/evaluation/data',
                            [bertje_name, robbert_name],
                            './synt_nl2i_eval_torch/evaluation/weights',
                            'cuda')
```
* Play around with the results as you see fit
* The code assumes you have generated grammars and data which you can generate using https://github.com/konstantinosKokos/metaclass-cfg

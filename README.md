# ProcessChat: A Dataset for Business Process Grounded Dialogs
This repository contains the ProcessChat dataset which accompanies the paper "ProcessChat: A Dataset for Business Process Grounded Dialogs" authored by Neelamadhav Gantayat, Avirup Saha and Renuka Sindhgatta in CODS 2025.

ProcessChat is a process-grounded dataset of conversations with a chatbot assistant that is designed to offer the following types of interactions to the user:

- Guide the user step-by-step through the process by providing details of the next step to execute having the context of the previous steps the user has been guided through.
- Ask the user to provide information when the process reaches an exclusive gateway to choose the relevant path and guide the user to the appropriate path
- Inform the user about the actor involved in performing the task
- Provide the user with the list of activities performed by an actor
- Inform the user on reaching the end of the process.

The user inputs including the chat context and expected chatbot assistant outputs in the train, validation and test sets are available in the following directories:
- `data`: contains train.jsonl, valid.jsonl and test.jsonl files for the complete dataset
- `data_no_constrainedpolicy`: contains train.jsonl, valid.jsonl and test.jsonl files for the dataset without the constrained natural language (CNL) policy rules
- `data_no_nlpolicy`: contains train.jsonl, valid.jsonl and test.jsonl files for the dataset without the natural language (NL) policy rules

## Attribution Notice

The ProcessChat dataset consists of conversations/dialogs between a user and an assistant. These conversations/dialogs were created by IBM based on BPMN process models and textual descriptions in a publicly available dataset at https://github.com/setzer22/alignment_model_text/tree/master/datasets which was released under the GPL v3 license: https://github.com/setzer22/alignment_model_text/blob/master/LICENSE. This dataset has been described by Sànchez-Ferreres *et al* in [1]. Consequently, while ProcessChat can be regarded as a “derivative” of the above dataset, it is significantly different because the conversations/dialogs in ProcessChat were not present in the above dataset. 
This data is being released purely for research purposes and not for any commercial use. No IP rights are associated with this dataset.

## References

[1] Sànchez-Ferreres, Josep, Han van der Aa, Josep Carmona, and Lluís Padró. "Aligning textual and model-based process descriptions." Data & Knowledge Engineering 118 (2018): 25-40.

[2] Sànchez-Ferreres, Josep, Josep Carmona, and Lluís Padró. "Aligning textual and graphical descriptions of processes through ILP techniques." In International Conference on Advanced Information Systems Engineering, pp. 413-427. Cham: Springer International Publishing, 2017. 

[3] Van der Aa, Han, Henrik Leopold, and Hajo A. Reijers. "Detecting inconsistencies between process models and textual descriptions." In International Conference on Business Process Management, pp. 90-105. Cham: Springer International Publishing, 2015.

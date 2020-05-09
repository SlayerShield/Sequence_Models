## Updates from Neural Machine Translation with Attention

### If you were working on the notebook before this update...
* The current notebook is version "4a".
* You can find your original work saved in the notebook with the previous version name ("v4") 
* To view the file directory, go to the menu "File->Open", and this will open a new tab that shows the file directory.

### List of updates
* Clarified names of variables to be consistent with the lectures and consistent within the assignment
    - pre-attention bi-directional LSTM: the first LSTM that processes the input data.
        - 'a': the hidden state of the pre-attention LSTM.
    - post-attention LSTM: the LSTM that outputs the translation.
        - 's': the hidden state of the post-attention LSTM.
    - energies "e".  The output of the dense function that takes "a" and "s" as inputs.
    - All references to "output activation" are updated to "hidden state".
    - "post-activation" sequence model is updated to "post-attention sequence model".
    - 3.1: "Getting the activations from the Network" renamed to "Getting the attention weights from the network."
    - Appropriate mentions of "activation" replaced "attention weights."
    - Sequence of alphas corrected to be a sequence of "a" hidden states.
* one_step_attention:
    - Provides sample code for each Keras layer, to show how to call the functions.
    - Reminds students to provide the list of hidden states in a specific order, in order to pause the autograder.
* model
    - Provides sample code for each Keras layer, to show how to call the functions.
    - Added a troubleshooting note about handling errors.
    - Fixed typo: outputs should be of length 10 and not 11.
* define optimizer and compile model
    - Provides sample code for each Keras layer, to show how to call the functions.

* Spelling, grammar and wording corrections.


## Updates from Trigger word detection

* 2.1: build the model
    * Added sample code to show how to use the Keras layers.
    * Lets student to implement the `TimeDistributed` code.
* Spelling, grammar and wording corrections.

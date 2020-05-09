## Updates from Building a Recurrent Neural Network Step by Step 

* "Forward propagation for the basic RNN", added sections to clarify variable names and shapes:
    - "Dimensions of $x^{\langle t \rangle}$"
    - "Hidden State $a$", 
    - "Dimensions of hidden state $a^{\langle t \rangle}$"
    - "Dimensions of prediction $y^{\langle t \rangle}$"
* `rnn_cell_forward`: 
    * Added additional hints.
    * Updated figure 2.
* `rnn_forward`
    - Set `xt` in a separate line of code to clarify what code is expected; added additional hints.
    - Clarifies instructions to specify dimensions (2D or 3D), and clarifies variable names.
    - Additional Hints
    - Clarifies when the basic RNN works well.
    - Updated figure 3.
* "About the gates" replaced with "overview of gates and states":
    - Updated to include conceptual description of each gate's purpose, and an explanation of each equation.  
    - Added sections about the cell state, hidden state, and prediction.
    - Lists variable names that are used in the code, and notes when they differ from the variables used in the equations.
    - Lists shapes of the variables.
    - Updated figure 4.
* `lstm_forward`
    - Added instructions, noting the shapes of the variables.
    - Added hints about `c` and `c_next` to help students avoid copy-by-reference mistakes.
    - Set `xt` in a separate line to make this step explicit.
* `dimension`
    - clarified use of $x^{(i)\langle t \rangle}$ in dimension description
* `Backward description`
    - Updated figure 6 and 7
* `rnn_cell_backward`
    - changed 'dtanh' to 'dz' to avoid confusion with the output of the tanh
    - fixed naming of 'b' in test section, changed to 'ba', updated results
* `rnn_backward`
    - modified instructions in comments to sum da and gradients from previous timesteps
* `lstm_cell_backward` 
    - updated equations and description to fix errors.
    - Added Figure 8
    - modified equations to use the term dlower_case_gamma vs dGamma - the previous naming confused the location of the gate derivative.    
    - removed redundant lines for equations 7-10, changed equation numbers to match new equation numbers
* `lstm_backward`
    - removed comment listing dc as argument.
    - added da_prevt and dc_prevt to for loop and recalculated results
    - in test, added "Wy" and "by" zero fill as it is required for lstm_forward. 
    
* Renamed global variables so that they do not conflict with local variables within the function.
* Spelling, grammar and wording corrections.
* For unit tests, updated print statements and "expected output" for easier comparisons.


## Updates from Building a recurrent neural network - step by step

* "Forward propagation for the basic RNN", added sections to clarify variable names and shapes:
    - "Dimensions of $x^{\langle t \rangle}$"
    - "Hidden State $a$", 
    - "Dimensions of hidden state $a^{\langle t \rangle}$"
    - "Dimensions of prediction $y^{\langle t \rangle}$"
* `rnn_cell_forward`: 
    * Added additional hints.
    * Updated figure 2.
* `rnn_forward`
    - Set `xt` in a separate line of code to clarify what code is expected; added additional hints.
    - Clarifies instructions to specify dimensions (2D or 3D), and clarifies variable names.
    - Additional Hints
    - Clarifies when the basic RNN works well.
    - Updated figure 3.
* "About the gates" replaced with "overview of gates and states":
    - Updated to include conceptual description of each gate's purpose, and an explanation of each equation.  
    - Added sections about the cell state, hidden state, and prediction.
    - Lists variable names that are used in the code, and notes when they differ from the variables used in the equations.
    - Lists shapes of the variables.
    - Updated figure 4.
* `lstm_forward`
    - Added instructions, noting the shapes of the variables.
    - Added hints about `c` and `c_next` to help students avoid copy-by-reference mistakes.
    - Set `xt` in a separate line to make this step explicit.
* `dimension`
    - clarified use of $x^{(i)\langle t \rangle}$ in dimension description
* `Backward description`
    - Updated figure 6 and 7
* `rnn_cell_backward`
    - changed 'dtanh' to 'dz' to avoid confusion with the output of the tanh
    - fixed naming of 'b' in test section, changed to 'ba', updated results
* `rnn_backward`
    - modified instructions in comments to sum da and gradients from previous timesteps
* `lstm_cell_backward` 
    - updated equations and description to fix errors.
    - Added Figure 8
    - modified equations to use the term dlower_case_gamma vs dGamma - the previous naming confused the location of the gate derivative.    
    - removed redundant lines for equations 7-10, changed equation numbers to match new equation numbers
* `lstm_backward`
    - removed comment listing dc as argument.
    - added da_prevt and dc_prevt to for loop and recalculated results
    - in test, added "Wy" and "by" zero fill as it is required for lstm_forward. 

* Renamed global variables so that they do not conflict with local variables within the function.
* Spelling, grammar and wording corrections.
* For unit tests, updated print statements and "expected output" for easier comparisons


## Updates from Jazz improvisation with LSTM

* `djmodel`
    - Explains `Input` layer and its parameter `shape`.
    - Explains `Lambda` layer and replaces the given solution with hints and sample code (to improve the learning experience).
    - Adds hints for using the Keras `Model`.
* `music_inference_model`
    - Explains each line of code in the `one_hot` function.
    - Explains how to apply `one_hot` with a Lambda layer instead of giving the code solution (to improve the learning experience).
    - Adds instructions on defining the `Model`.
* `predict_and_sample`
    - Provides detailed instructions for each step.
    - Clarifies which variable/function to use for inference.
* Spelling, grammar and wording corrections.

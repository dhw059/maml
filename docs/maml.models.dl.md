---
layout: default
title: maml.models.dl.md
nav_exclude: true
---

# maml.models.dl package

Deep learning module.

## *class* maml.models.dl.AtomSets(describer: BaseDescriber | None = None, input_dim: int | None = None, is_embedding: bool = True, n_neurons: Sequence[int] = (64, 64), n_neurons_final: Sequence[int] = (64, 64), n_targets: int = 1, activation: str = ‘relu’, embedding_vcal: int = 95, embedding_dim: int = 32, symmetry_func: list[str] | str = ‘mean’, optimizer: str = ‘adam’, loss: str = ‘mse’, compile_metrics: tuple = (), is_classification: bool = False, \*\*symmetry_func_kwargs)

Bases: `KerasModel`

This class implements the DeepSets models.

### _get_data_generator(features, targets, batch_size=128, is_shuffle=True)

### _predict(features: ndarray, \*\*kwargs)

Predict the values given a set of inputs based on fitted models.


* **Parameters**
**features** (*np.ndarray*) – array-like input features.


* **Returns**
List of output objects.

### evaluate(eval_objs, eval_targets, is_feature: bool = False, batch_size: int = 16)

Evaluate objs, targets.


* **Parameters**

    * **eval_objs** (*list*) – objs for evaluation


    * **eval_targets** (*list*) – target list for the corresponding objects


    * **is_feature** (*bool*) – whether x is feature matrix


    * **batch_size** (*int*) – evaluation batch size

### fit(features: list | np.ndarray, targets: list | np.ndarray | None = None, val_features: list | np.ndarray | None = None, val_targets: list | np.ndarray | None = None, \*\*kwargs)


* **Parameters**

    * **features** (*list*\* or \**np.ndarray*) – Numerical input feature list or
numpy array with dim (m, n) where m is the number of data and
n is the feature dimension.


    * **targets** (*list*\* or \**np.ndarray*) – Numerical output target list, or
numpy array with dim (m, ).


    * **val_features** (*list*\* or \**np.ndarray*) – validation features


    * **val_targets** (*list*\* or \**np.ndarray*) – validation targets.

### *classmethod* from_dir(dirname: str)

Load the models from file
:param dirname: directory name
:type dirname: str

Returns: object instance.

### save(dirname: str)

Save the models and describers.


* **Parameters**
**dirname** (*str*) – dirname for save

## *class* maml.models.dl.MLP(input_dim: int | None = None, describer: BaseDescriber | None = None, n_neurons: tuple = (64, 64), activation: str = ‘relu’, n_targets: int = 1, is_classification: bool = False, optimizer: str = ‘adam’, loss: str = ‘mse’, compile_metrics: tuple = (), \*\*kwargs)

Bases: `KerasModel`

This class implements the multi-layer perceptron models.

## *class* maml.models.dl.WeightedAverageLayer(\*args, \*\*kwargs)

Bases: `Layer`

Weight average the features using weights.

result= sum{w_i^a \* value_i} / sum{w_i^a}

### build(input_shape: Sequence)

Build the layer.


* **Parameters**
**input_shape** (*tuple*) – input shape tuple

### call(inputs: Sequence, mask: tf.Tensor | None = None)

Core logic of the layer.


* **Parameters**

    * **inputs** (*tuple*) – input tuple of length 3


    * **mask** (*tf.Tensor*) – not used here

### *static* compute_output_shape(input_shape: Sequence)

Compute output shape from input shape
:param input_shape: input shape list.
:type input_shape: tuple/list

### get_config()

Get layer configuration.

### *static* reduce_sum(prop: Tensor, index: Tensor, perm: Sequence)

Reduce sum the tensors using index.


* **Parameters**

    * **prop** (*tf.Tensor*) – tensor with shape [1, n, …]


    * **index** (*tf.Tensor*) – integer tensor with shape [1, n]


    * **perm** (*list*) – permutation for transpose.

## *class* maml.models.dl.WeightedSet2Set(\*args, \*\*kwargs)

Bases: `Layer`

This is a modified version from megnet.layers.readout.Set2Set.
Here, in addition to taking features and indices as inputs, we also
take a weight tensor. The input to the core logic is
[features, weights, indices].

### _lstm(h, c)

### build(input_shape: Sequence)

Build the output shape from input shapes
:param input_shape: input shape list.
:type input_shape: tuple/list

### call(inputs, mask=None)

Core logic of the layer.


* **Parameters**

    * **inputs** (*tuple*) – input tuple of length 3


    * **mask** (*tf.Tensor*) – not used here

### compute_output_shape(input_shape)

Compute output shapes from input shapes
:param input_shape: input shapes.
:type input_shape: sequence of tuple

Returns: sequence of tuples output shapes

### get_config()

> Part of keras layer interface, where the signature is converted into a dict


* **Returns**
configurational dictionary.

## maml.models.dl._atomsets module

neural network models.

### *class* maml.models.dl._atomsets.AtomSets(describer: BaseDescriber | None = None, input_dim: int | None = None, is_embedding: bool = True, n_neurons: Sequence[int] = (64, 64), n_neurons_final: Sequence[int] = (64, 64), n_targets: int = 1, activation: str = ‘relu’, embedding_vcal: int = 95, embedding_dim: int = 32, symmetry_func: list[str] | str = ‘mean’, optimizer: str = ‘adam’, loss: str = ‘mse’, compile_metrics: tuple = (), is_classification: bool = False, \*\*symmetry_func_kwargs)

Bases: `KerasModel`

This class implements the DeepSets models.

#### _get_data_generator(features, targets, batch_size=128, is_shuffle=True)

#### _predict(features: ndarray, \*\*kwargs)

Predict the values given a set of inputs based on fitted models.


* **Parameters**
**features** (*np.ndarray*) – array-like input features.


* **Returns**
List of output objects.

#### evaluate(eval_objs, eval_targets, is_feature: bool = False, batch_size: int = 16)

Evaluate objs, targets.


* **Parameters**

    * **eval_objs** (*list*) – objs for evaluation


    * **eval_targets** (*list*) – target list for the corresponding objects


    * **is_feature** (*bool*) – whether x is feature matrix


    * **batch_size** (*int*) – evaluation batch size

#### fit(features: list | np.ndarray, targets: list | np.ndarray | None = None, val_features: list | np.ndarray | None = None, val_targets: list | np.ndarray | None = None, \*\*kwargs)


* **Parameters**

    * **features** (*list*\* or \**np.ndarray*) – Numerical input feature list or
numpy array with dim (m, n) where m is the number of data and
n is the feature dimension.


    * **targets** (*list*\* or \**np.ndarray*) – Numerical output target list, or
numpy array with dim (m, ).


    * **val_features** (*list*\* or \**np.ndarray*) – validation features


    * **val_targets** (*list*\* or \**np.ndarray*) – validation targets.

#### *classmethod* from_dir(dirname: str)

Load the models from file
:param dirname: directory name
:type dirname: str

Returns: object instance.

#### save(dirname: str)

Save the models and describers.


* **Parameters**
**dirname** (*str*) – dirname for save

### maml.models.dl._atomsets.construct_atom_sets(input_dim: int | None = None, is_embedding: bool = True, n_neurons: Sequence[int] = (64, 64), n_neurons_final: Sequence[int] = (64, 64), n_targets: int = 1, activation: str = ‘relu’, embedding_vcal: int = 95, embedding_dim: int = 32, symmetry_func: list[str] | str = ‘mean’, optimizer: str = ‘adam’, loss: str = ‘mse’, compile_metrics: tuple = (), is_classification: bool = False, \*\*symmetry_func_kwargs)

f(X) = rho(sum_{x in X} phi(x)), where X is a set.
phi is implemented as a neural network and rho is a symmetry function.

todo: implement attention mechanism


* **Parameters**

    * **input_dim** (*int*) – input dimension, if None, then integer inputs + embedding are assumed.


    * **is_embedding** (*bool*) – whether the input should be embedded


    * **n_neurons** (*tuple*) – number of hidden-layer neurons before passing to symmetry function


    * **n_neurons_final** (*tuple*) – number of hidden-layer neurons after symmetry function


    * **n_targets** (*int*) – number of output targets


    * **activation** (*str*) – activation function


    * **embedding_vcal** (*int*) – int, embedding vocabulary


    * **embedding_dim** (*int*) – int, embedding dimension


    * **symmetry_func** (*str*) – symmetry function, choose from [‘set2set’, ‘sum’, ‘mean’,
‘max’, ‘min’, ‘prod’]


    * **optimizer** (*str*) – optimizer for the models


    * **loss** (*str*) – loss function for the models


    * **compile_metrics** (*tuple*) – metrics for validation


    * **symmetry_func_kwargs** (*dict*) – kwargs for symmetry function

## maml.models.dl._keras_utils module

Keras utils for deserialize activations and otpimizers.

### maml.models.dl._keras_utils.deserialize_keras_activation(activation)

serialize keras activation.


* **Parameters**
**activation** (*str*\*, **dict**, or \**Activation object*) – activation to serialize

Returns: Activation object

### maml.models.dl._keras_utils.deserialize_keras_optimizer(optimizer)

serialize keras activation.


* **Parameters**
**optimizer** (*str*\*, **dict**, or \**optimizer object*) – optimizer to serialize

Returns: Activation object

## maml.models.dl._layers module

Deep learning layers.

### *class* maml.models.dl._layers.WeightedAverageLayer(\*args, \*\*kwargs)

Bases: `Layer`

Weight average the features using weights.

result= sum{w_i^a \* value_i} / sum{w_i^a}

#### build(input_shape: Sequence)

Build the layer.


* **Parameters**
**input_shape** (*tuple*) – input shape tuple

#### call(inputs: Sequence, mask: tf.Tensor | None = None)

Core logic of the layer.


* **Parameters**

    * **inputs** (*tuple*) – input tuple of length 3


    * **mask** (*tf.Tensor*) – not used here

#### *static* compute_output_shape(input_shape: Sequence)

Compute output shape from input shape
:param input_shape: input shape list.
:type input_shape: tuple/list

#### get_config()

Get layer configuration.

#### *static* reduce_sum(prop: Tensor, index: Tensor, perm: Sequence)

Reduce sum the tensors using index.


* **Parameters**

    * **prop** (*tf.Tensor*) – tensor with shape [1, n, …]


    * **index** (*tf.Tensor*) – integer tensor with shape [1, n]


    * **perm** (*list*) – permutation for transpose.

### *class* maml.models.dl._layers.WeightedSet2Set(\*args, \*\*kwargs)

Bases: `Layer`

This is a modified version from megnet.layers.readout.Set2Set.
Here, in addition to taking features and indices as inputs, we also
take a weight tensor. The input to the core logic is
[features, weights, indices].

#### _lstm(h, c)

#### build(input_shape: Sequence)

Build the output shape from input shapes
:param input_shape: input shape list.
:type input_shape: tuple/list

#### call(inputs, mask=None)

Core logic of the layer.


* **Parameters**

    * **inputs** (*tuple*) – input tuple of length 3


    * **mask** (*tf.Tensor*) – not used here

#### compute_output_shape(input_shape)

Compute output shapes from input shapes
:param input_shape: input shapes.
:type input_shape: sequence of tuple

Returns: sequence of tuples output shapes

#### get_config()

> Part of keras layer interface, where the signature is converted into a dict


* **Returns**
configurational dictionary.

## maml.models.dl._mlp module

Multi-layer perceptron models.

### *class* maml.models.dl._mlp.MLP(input_dim: int | None = None, describer: BaseDescriber | None = None, n_neurons: tuple = (64, 64), activation: str = ‘relu’, n_targets: int = 1, is_classification: bool = False, optimizer: str = ‘adam’, loss: str = ‘mse’, compile_metrics: tuple = (), \*\*kwargs)

Bases: `KerasModel`

This class implements the multi-layer perceptron models.

### maml.models.dl._mlp.construct_mlp(input_dim: int, n_neurons: tuple = (64, 64), activation: str = ‘relu’, n_targets: int = 1, is_classification: bool = False, optimizer: str = ‘adam’, loss: str = ‘mse’, compile_metrics: tuple = ())

Constructor for multi-layer perceptron models.


* **Parameters**

    * **input_dim** (*int*) – input dimension, i.e., feature dimension


    * **n_neurons** (*tuple*) – list of hidden neuron sizes


    * **activation** (*str*) – activation function


    * **n_targets** (*int*) – number of targets


    * **is_classification** (*bool*) – whether the target is a classification problem


    * **optimizer** (*str*) – optimizer


    * **loss** (*str*) – loss function


    * **compile_metrics** (*tuple*) – metrics to evaluate during epochs
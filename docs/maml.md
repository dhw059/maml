---
layout: default
title: API Documentation
nav_order: 5
---

# maml package

## Subpackages


* [maml.apps package](maml.apps.md)


    * Subpackages


        * [maml.apps.bowsr package](maml.apps.bowsr.md)


            * Subpackages


                * [maml.apps.bowsr.model package](maml.apps.bowsr.model.md)


                    * `EnergyModel`


                    * maml.apps.bowsr.model.base module


                    * maml.apps.bowsr.model.cgcnn module


                    * maml.apps.bowsr.model.dft module


                    * maml.apps.bowsr.model.megnet module


            * maml.apps.bowsr.acquisition module


                * `AcquisitionFunction`


                    * `AcquisitionFunction._ei()`


                    * `AcquisitionFunction._gpucb()`


                    * `AcquisitionFunction._poi()`


                    * `AcquisitionFunction._ucb()`


                    * `AcquisitionFunction.calculate()`


                * `_trunc()`


                * `ensure_rng()`


                * `lhs_sample()`


                * `predict_mean_std()`


                * `propose_query_point()`


            * maml.apps.bowsr.optimizer module


                * `BayesianOptimizer`


                    * `BayesianOptimizer.add_query()`


                    * `BayesianOptimizer.as_dict()`


                    * `BayesianOptimizer.from_dict()`


                    * `BayesianOptimizer.get_derived_structure()`


                    * `BayesianOptimizer.get_formation_energy()`


                    * `BayesianOptimizer.get_optimized_structure_and_energy()`


                    * `BayesianOptimizer.gpr`


                    * `BayesianOptimizer.optimize()`


                    * `BayesianOptimizer.propose()`


                    * `BayesianOptimizer.set_bounds()`


                    * `BayesianOptimizer.set_gpr_params()`


                    * `BayesianOptimizer.set_space_empty()`


                    * `BayesianOptimizer.space`


                * `atoms_crowded()`


                * `struct2perturbation()`


            * maml.apps.bowsr.perturbation module


                * `LatticePerturbation`


                    * `LatticePerturbation.abc`


                    * `LatticePerturbation.fit_lattice`


                    * `LatticePerturbation.lattice`


                    * `LatticePerturbation.sanity_check()`


                * `WyckoffPerturbation`


                    * `WyckoffPerturbation.fit_site`


                    * `WyckoffPerturbation.get_orbit()`


                    * `WyckoffPerturbation.sanity_check()`


                    * `WyckoffPerturbation.site`


                    * `WyckoffPerturbation.standardize()`


                * `crystal_system()`


                * `get_standardized_structure()`


                * `perturbation_mapping()`


            * maml.apps.bowsr.preprocessing module


                * `DummyScaler`


                    * `DummyScaler.as_dict()`


                    * `DummyScaler.fit()`


                    * `DummyScaler.from_dict()`


                    * `DummyScaler.inverse_transform()`


                    * `DummyScaler.transform()`


                * `StandardScaler`


                    * `StandardScaler.as_dict()`


                    * `StandardScaler.fit()`


                    * `StandardScaler.from_dict()`


                    * `StandardScaler.inverse_transform()`


                    * `StandardScaler.transform()`


            * maml.apps.bowsr.target_space module


                * `TargetSpace`


                    * `TargetSpace.bounds`


                    * `TargetSpace.lhs_sample()`


                    * `TargetSpace.params`


                    * `TargetSpace.probe()`


                    * `TargetSpace.register()`


                    * `TargetSpace.set_bounds()`


                    * `TargetSpace.set_empty()`


                    * `TargetSpace.target`


                    * `TargetSpace.uniform_sample()`


                * `_hashable()`


        * [maml.apps.gbe package](maml.apps.gbe.md)


            * maml.apps.gbe.describer module


                * `GBBond`


                    * `GBBond.NNDict`


                    * `GBBond._get_bond_mat()`


                    * `GBBond.as_dict()`


                    * `GBBond.bond_matrix`


                    * `GBBond.from_dict()`


                    * `GBBond.get_breakbond_ratio()`


                    * `GBBond.get_mean_bl_chg()`


                    * `GBBond.max_bl`


                    * `GBBond.min_bl`


                * `GBDescriber`


                    * `GBDescriber._abc_impl`


                    * `GBDescriber._sklearn_auto_wrap_output_keys`


                    * `GBDescriber.generate_bulk_ref()`


                    * `GBDescriber.transform_one()`


                * `convert_hcp_direction()`


                * `convert_hcp_plane()`


                * `get_elemental_feature()`


                * `get_structural_feature()`


            * maml.apps.gbe.presetfeatures module


                * `my_quant`


                    * `my_quant.latex`


                    * `my_quant.name`


                    * `my_quant.unit`


            * maml.apps.gbe.utils module


                * `load_b0_dict()`


                * `load_data()`


                * `load_mean_delta_bl_dict()`


                * `update_b0_dict()`


        * [maml.apps.pes package](maml.apps.pes.md)


            * `DefectFormation`


                * `DefectFormation._parse()`


                * `DefectFormation._sanity_check()`


                * `DefectFormation._setup()`


                * `DefectFormation.calculate()`


                * `DefectFormation.get_unit_cell()`


            * `ElasticConstant`


                * `ElasticConstant._RESTART_CONFIG`


                * `ElasticConstant._parse()`


                * `ElasticConstant._sanity_check()`


                * `ElasticConstant._setup()`


            * `EnergyForceStress`


                * `EnergyForceStress._parse()`


                * `EnergyForceStress._rotate_force_stress()`


                * `EnergyForceStress._sanity_check()`


                * `EnergyForceStress._setup()`


                * `EnergyForceStress.calculate()`


            * `GAPotential`


                * `GAPotential._abc_impl`


                * `GAPotential._line_up()`


                * `GAPotential.evaluate()`


                * `GAPotential.from_config()`


                * `GAPotential.pair_coeff`


                * `GAPotential.pair_style`


                * `GAPotential.read_cfgs()`


                * `GAPotential.save()`


                * `GAPotential.train()`


                * `GAPotential.write_cfgs()`


                * `GAPotential.write_param()`


            * `LMPStaticCalculator`


                * `LMPStaticCalculator._COMMON_CMDS`


                * `LMPStaticCalculator._parse()`


                * `LMPStaticCalculator._sanity_check()`


                * `LMPStaticCalculator._setup()`


                * `LMPStaticCalculator.allowed_kwargs`


                * `LMPStaticCalculator.calculate()`


                * `LMPStaticCalculator.set_lmp_exe()`


            * `LatticeConstant`


                * `LatticeConstant.calculate()`


            * `MTPotential`


                * `MTPotential._abc_impl`


                * `MTPotential._line_up()`


                * `MTPotential.evaluate()`


                * `MTPotential.from_config()`


                * `MTPotential.pair_coeff`


                * `MTPotential.pair_style`


                * `MTPotential.read_cfgs()`


                * `MTPotential.train()`


                * `MTPotential.write_cfg()`


                * `MTPotential.write_ini()`


                * `MTPotential.write_param()`


            * `NNPotential`


                * `NNPotential._abc_impl`


                * `NNPotential._line_up()`


                * `NNPotential.bohr_to_angstrom`


                * `NNPotential.eV_to_Ha`


                * `NNPotential.evaluate()`


                * `NNPotential.from_config()`


                * `NNPotential.load_input()`


                * `NNPotential.load_scaler()`


                * `NNPotential.load_weights()`


                * `NNPotential.pair_coeff`


                * `NNPotential.pair_style`


                * `NNPotential.read_cfgs()`


                * `NNPotential.train()`


                * `NNPotential.write_cfgs()`


                * `NNPotential.write_input()`


                * `NNPotential.write_param()`


            * `NudgedElasticBand`


                * `NudgedElasticBand._parse()`


                * `NudgedElasticBand._sanity_check()`


                * `NudgedElasticBand._setup()`


                * `NudgedElasticBand.calculate()`


                * `NudgedElasticBand.get_unit_cell()`


            * `Potential`


            * `SNAPotential`


                * `SNAPotential._abc_impl`


                * `SNAPotential.evaluate()`


                * `SNAPotential.from_config()`


                * `SNAPotential.pair_coeff`


                * `SNAPotential.pair_style`


                * `SNAPotential.train()`


                * `SNAPotential.write_param()`


            * `SpectralNeighborAnalysis`


                * `SpectralNeighborAnalysis._CMDS`


                * `SpectralNeighborAnalysis._parse()`


                * `SpectralNeighborAnalysis._sanity_check()`


                * `SpectralNeighborAnalysis._setup()`


                * `SpectralNeighborAnalysis.get_bs_subscripts()`


                * `SpectralNeighborAnalysis.n_bs`


            * `get_default_lmp_exe()`


            * maml.apps.pes._base module


                * `Potential`


                * `PotentialMixin`


                    * `PotentialMixin.evaluate()`


                    * `PotentialMixin.from_config()`


                    * `PotentialMixin.predict_efs()`


                    * `PotentialMixin.train()`


                    * `PotentialMixin.write_param()`


            * maml.apps.pes._gap module


                * `GAPotential`


                    * `GAPotential._abc_impl`


                    * `GAPotential._line_up()`


                    * `GAPotential.evaluate()`


                    * `GAPotential.from_config()`


                    * `GAPotential.pair_coeff`


                    * `GAPotential.pair_style`


                    * `GAPotential.read_cfgs()`


                    * `GAPotential.save()`


                    * `GAPotential.train()`


                    * `GAPotential.write_cfgs()`


                    * `GAPotential.write_param()`


            * maml.apps.pes._lammps module


                * `DefectFormation`


                    * `DefectFormation._parse()`


                    * `DefectFormation._sanity_check()`


                    * `DefectFormation._setup()`


                    * `DefectFormation.calculate()`


                    * `DefectFormation.get_unit_cell()`


                * `ElasticConstant`


                    * `ElasticConstant._RESTART_CONFIG`


                    * `ElasticConstant._parse()`


                    * `ElasticConstant._sanity_check()`


                    * `ElasticConstant._setup()`


                * `EnergyForceStress`


                    * `EnergyForceStress._parse()`


                    * `EnergyForceStress._rotate_force_stress()`


                    * `EnergyForceStress._sanity_check()`


                    * `EnergyForceStress._setup()`


                    * `EnergyForceStress.calculate()`


                * `LMPRelaxationCalculator`


                    * `LMPRelaxationCalculator._parse()`


                    * `LMPRelaxationCalculator._sanity_check()`


                    * `LMPRelaxationCalculator._setup()`


                * `LMPStaticCalculator`


                    * `LMPStaticCalculator._COMMON_CMDS`


                    * `LMPStaticCalculator._parse()`


                    * `LMPStaticCalculator._sanity_check()`


                    * `LMPStaticCalculator._setup()`


                    * `LMPStaticCalculator.allowed_kwargs`


                    * `LMPStaticCalculator.calculate()`


                    * `LMPStaticCalculator.set_lmp_exe()`


                * `LammpsPotential`


                    * `LammpsPotential._abc_impl`


                    * `LammpsPotential.predict_efs()`


                * `LatticeConstant`


                    * `LatticeConstant.calculate()`


                * `NudgedElasticBand`


                    * `NudgedElasticBand._parse()`


                    * `NudgedElasticBand._sanity_check()`


                    * `NudgedElasticBand._setup()`


                    * `NudgedElasticBand.calculate()`


                    * `NudgedElasticBand.get_unit_cell()`


                * `SpectralNeighborAnalysis`


                    * `SpectralNeighborAnalysis._CMDS`


                    * `SpectralNeighborAnalysis._parse()`


                    * `SpectralNeighborAnalysis._sanity_check()`


                    * `SpectralNeighborAnalysis._setup()`


                    * `SpectralNeighborAnalysis.get_bs_subscripts()`


                    * `SpectralNeighborAnalysis.n_bs`


                * `SurfaceEnergy`


                    * `SurfaceEnergy.calculate()`


                * `_pretty_input()`


                * `_read_dump()`


                * `get_default_lmp_exe()`


            * maml.apps.pes._mtp module


                * `MTPotential`


                    * `MTPotential._abc_impl`


                    * `MTPotential._line_up()`


                    * `MTPotential.evaluate()`


                    * `MTPotential.from_config()`


                    * `MTPotential.pair_coeff`


                    * `MTPotential.pair_style`


                    * `MTPotential.read_cfgs()`


                    * `MTPotential.train()`


                    * `MTPotential.write_cfg()`


                    * `MTPotential.write_ini()`


                    * `MTPotential.write_param()`


                * `feed()`


            * maml.apps.pes._nnp module


                * `NNPotential`


                    * `NNPotential._abc_impl`


                    * `NNPotential._line_up()`


                    * `NNPotential.bohr_to_angstrom`


                    * `NNPotential.eV_to_Ha`


                    * `NNPotential.evaluate()`


                    * `NNPotential.from_config()`


                    * `NNPotential.load_input()`


                    * `NNPotential.load_scaler()`


                    * `NNPotential.load_weights()`


                    * `NNPotential.pair_coeff`


                    * `NNPotential.pair_style`


                    * `NNPotential.read_cfgs()`


                    * `NNPotential.train()`


                    * `NNPotential.write_cfgs()`


                    * `NNPotential.write_input()`


                    * `NNPotential.write_param()`


            * maml.apps.pes._snap module


                * `SNAPotential`


                    * `SNAPotential._abc_impl`


                    * `SNAPotential.evaluate()`


                    * `SNAPotential.from_config()`


                    * `SNAPotential.pair_coeff`


                    * `SNAPotential.pair_style`


                    * `SNAPotential.train()`


                    * `SNAPotential.write_param()`


        * [maml.apps.symbolic package](maml.apps.symbolic.md)


            * `AdaptiveLasso`


                * `AdaptiveLasso._penalty_jac()`


                * `AdaptiveLasso.get_w()`


                * `AdaptiveLasso.penalty()`


                * `AdaptiveLasso.select()`


            * `DantzigSelector`


                * `DantzigSelector.construct_constraints()`


                * `DantzigSelector.construct_jac()`


                * `DantzigSelector.construct_loss()`


            * `FeatureGenerator`


                * `FeatureGenerator.augment()`


            * `ISIS`


                * `ISIS.evaluate()`


                * `ISIS.run()`


            * `L0BrutalForce`


                * `L0BrutalForce.select()`


            * `Lasso`


                * `Lasso._penalty_jac()`


                * `Lasso.penalty()`


            * `Operator`


                * `Operator.compute()`


                * `Operator.from_str()`


                * `Operator.gen_name()`


                * `Operator.is_binary`


                * `Operator.is_commutative`


                * `Operator.is_unary`


                * `Operator.support_op_rep`


            * `SCAD`


                * `SCAD._penalty_jac()`


                * `SCAD.penalty()`


            * `SIS`


                * `SIS.compute_residual()`


                * `SIS.run()`


                * `SIS.screen()`


                * `SIS.select()`


                * `SIS.set_gamma()`


                * `SIS.set_selector()`


                * `SIS.update_gamma()`


            * maml.apps.symbolic._feature_generator module


                * `FeatureGenerator`


                    * `FeatureGenerator.augment()`


                * `Operator`


                    * `Operator.compute()`


                    * `Operator.from_str()`


                    * `Operator.gen_name()`


                    * `Operator.is_binary`


                    * `Operator.is_commutative`


                    * `Operator.is_unary`


                    * `Operator.support_op_rep`


                * `_my_abs_diff()`


                * `_my_abs_log10()`


                * `_my_abs_sqrt()`


                * `_my_abs_sum()`


                * `_my_diff()`


                * `_my_div()`


                * `_my_exp()`


                * `_my_exp_power_2()`


                * `_my_exp_power_3()`


                * `_my_mul()`


                * `_my_power()`


                * `_my_sum()`


                * `_my_sum_exp()`


                * `_my_sum_power_2()`


                * `_my_sum_power_3()`


                * `_update_df()`


                * `generate_feature()`


            * maml.apps.symbolic._selectors module


                * `AdaptiveLasso`


                    * `AdaptiveLasso._penalty_jac()`


                    * `AdaptiveLasso.get_w()`


                    * `AdaptiveLasso.penalty()`


                    * `AdaptiveLasso.select()`


                * `BaseSelector`


                    * `BaseSelector._get_param_names()`


                    * `BaseSelector.compute_residual()`


                    * `BaseSelector.construct_constraints()`


                    * `BaseSelector.construct_jac()`


                    * `BaseSelector.construct_loss()`


                    * `BaseSelector.evaluate()`


                    * `BaseSelector.get_coef()`


                    * `BaseSelector.get_feature_indices()`


                    * `BaseSelector.get_params()`


                    * `BaseSelector.predict()`


                    * `BaseSelector.select()`


                    * `BaseSelector.set_params()`


                * `DantzigSelector`


                    * `DantzigSelector.construct_constraints()`


                    * `DantzigSelector.construct_jac()`


                    * `DantzigSelector.construct_loss()`


                * `L0BrutalForce`


                    * `L0BrutalForce.select()`


                * `Lasso`


                    * `Lasso._penalty_jac()`


                    * `Lasso.penalty()`


                * `PenalizedLeastSquares`


                    * `PenalizedLeastSquares._penalty_jac()`


                    * `PenalizedLeastSquares._sse_jac()`


                    * `PenalizedLeastSquares.construct_constraints()`


                    * `PenalizedLeastSquares.construct_jac()`


                    * `PenalizedLeastSquares.construct_loss()`


                    * `PenalizedLeastSquares.penalty()`


                * `SCAD`


                    * `SCAD._penalty_jac()`


                    * `SCAD.penalty()`


            * maml.apps.symbolic._selectors_cvxpy module


                * `AdaptiveLassoCP`


                    * `AdaptiveLassoCP.get_w()`


                    * `AdaptiveLassoCP.penalty()`


                    * `AdaptiveLassoCP.select()`


                * `BaseSelectorCP`


                    * `BaseSelectorCP.construct_constraints()`


                    * `BaseSelectorCP.construct_loss()`


                    * `BaseSelectorCP.select()`


                * `DantzigSelectorCP`


                    * `DantzigSelectorCP.construct_constraints()`


                    * `DantzigSelectorCP.construct_loss()`


                * `LassoCP`


                    * `LassoCP.penalty()`


                * `PenalizedLeastSquaresCP`


                    * `PenalizedLeastSquaresCP.construct_loss()`


                    * `PenalizedLeastSquaresCP.penalty()`


            * maml.apps.symbolic._sis module


                * `ISIS`


                    * `ISIS.evaluate()`


                    * `ISIS.run()`


                * `SIS`


                    * `SIS.compute_residual()`


                    * `SIS.run()`


                    * `SIS.screen()`


                    * `SIS.select()`


                    * `SIS.set_gamma()`


                    * `SIS.set_selector()`


                    * `SIS.update_gamma()`


                * `_best_combination()`


                * `_eval()`


                * `_get_coeff()`


* [maml.base package](maml.base.md)


    * `BaseDataSource`


        * `BaseDataSource.get()`


    * `BaseDescriber`


        * `BaseDescriber._abc_impl`


        * `BaseDescriber._is_multi_output()`


        * `BaseDescriber._sklearn_auto_wrap_output_keys`


        * `BaseDescriber.clear_cache()`


        * `BaseDescriber.feature_dim`


        * `BaseDescriber.fit()`


        * `BaseDescriber.transform()`


        * `BaseDescriber.transform_one()`


    * `BaseModel`


        * `BaseModel._predict()`


        * `BaseModel.fit()`


        * `BaseModel.predict_objs()`


        * `BaseModel.train()`


    * `DummyDescriber`


        * `DummyDescriber._abc_impl`


        * `DummyDescriber._sklearn_auto_wrap_output_keys`


        * `DummyDescriber.transform_one()`


    * `KerasModel`


        * `KerasModel._get_validation_data()`


        * `KerasModel.fit()`


    * `SKLModel`


    * `SequentialDescriber`


        * `SequentialDescriber._abc_impl`


        * `SequentialDescriber.steps`


    * `TargetScalerMixin`


        * `TargetScalerMixin.predict_objs()`


        * `TargetScalerMixin.train()`


    * `describer_type()`


    * `get_feature_batch()`


    * `is_keras_model()`


    * `is_sklearn_model()`


    * maml.base._data module


        * `BaseDataSource`


            * `BaseDataSource.get()`


    * maml.base._describer module


        * `BaseDescriber`


            * `BaseDescriber._abc_impl`


            * `BaseDescriber._is_multi_output()`


            * `BaseDescriber._sklearn_auto_wrap_output_keys`


            * `BaseDescriber.clear_cache()`


            * `BaseDescriber.feature_dim`


            * `BaseDescriber.fit()`


            * `BaseDescriber.transform()`


            * `BaseDescriber.transform_one()`


        * `DummyDescriber`


            * `DummyDescriber._abc_impl`


            * `DummyDescriber._sklearn_auto_wrap_output_keys`


            * `DummyDescriber.transform_one()`


        * `SequentialDescriber`


            * `SequentialDescriber._abc_impl`


            * `SequentialDescriber.steps`


        * `_transform_one()`


        * `describer_type()`


    * maml.base._feature_batch module


        * `get_feature_batch()`


        * `no_action()`


        * `pandas_concat()`


        * `stack_first_dim()`


        * `stack_padded()`


    * maml.base._mixin module


        * `TargetScalerMixin`


            * `TargetScalerMixin.predict_objs()`


            * `TargetScalerMixin.train()`


    * maml.base._model module


        * `BaseModel`


            * `BaseModel._predict()`


            * `BaseModel.fit()`


            * `BaseModel.predict_objs()`


            * `BaseModel.train()`


        * `KerasMixin`


            * `KerasMixin.evaluate()`


            * `KerasMixin.from_file()`


            * `KerasMixin.get_input_dim()`


            * `KerasMixin.load()`


            * `KerasMixin.save()`


        * `KerasModel`


            * `KerasModel._get_validation_data()`


            * `KerasModel.fit()`


        * `SKLModel`


        * `SklearnMixin`


            * `SklearnMixin.evaluate()`


            * `SklearnMixin.from_file()`


            * `SklearnMixin.load()`


            * `SklearnMixin.save()`


        * `is_keras_model()`


        * `is_sklearn_model()`


* [maml.data package](maml.data.md)


    * `MaterialsProject`


        * `MaterialsProject.get()`


    * `URLSource`


        * `URLSource.get()`


    * maml.data._mp module


        * `MaterialsProject`


            * `MaterialsProject.get()`


    * maml.data._url module


        * `FigshareSource`


            * `FigshareSource.get()`


        * `URLSource`


            * `URLSource.get()`


* [maml.describers package](maml.describers.md)


    * `BPSymmetryFunctions`


        * `BPSymmetryFunctions._abc_impl`


        * `BPSymmetryFunctions._fc()`


        * `BPSymmetryFunctions._sklearn_auto_wrap_output_keys`


        * `BPSymmetryFunctions.describer_type`


        * `BPSymmetryFunctions.transform_one()`


    * `BispectrumCoefficients`


        * `BispectrumCoefficients._abc_impl`


        * `BispectrumCoefficients._sklearn_auto_wrap_output_keys`


        * `BispectrumCoefficients.describer_type`


        * `BispectrumCoefficients.feature_dim`


        * `BispectrumCoefficients.subscripts`


        * `BispectrumCoefficients.transform_one()`


    * `CoulombEigenSpectrum`


        * `CoulombEigenSpectrum._abc_impl`


        * `CoulombEigenSpectrum._sklearn_auto_wrap_output_keys`


        * `CoulombEigenSpectrum.describer_type`


        * `CoulombEigenSpectrum.transform_one()`


    * `CoulombMatrix`


        * `CoulombMatrix._abc_impl`


        * `CoulombMatrix._get_columb_mat()`


        * `CoulombMatrix._sklearn_auto_wrap_output_keys`


        * `CoulombMatrix.describer_type`


        * `CoulombMatrix.get_coulomb_mat()`


        * `CoulombMatrix.transform_one()`


    * `DistinctSiteProperty`


        * `DistinctSiteProperty._abc_impl`


        * `DistinctSiteProperty._sklearn_auto_wrap_output_keys`


        * `DistinctSiteProperty.describer_type`


        * `DistinctSiteProperty.supported_properties`


        * `DistinctSiteProperty.transform_one()`


    * `ElementProperty`


        * `ElementProperty._abc_impl`


        * `ElementProperty._get_param_names()`


        * `ElementProperty._sklearn_auto_wrap_output_keys`


        * `ElementProperty.describer_type`


        * `ElementProperty.from_preset()`


        * `ElementProperty.get_params()`


        * `ElementProperty.transform_one()`


    * `ElementStats`


        * `ElementStats.ALLOWED_STATS`


        * `ElementStats.AVAILABLE_DATA`


        * `ElementStats._abc_impl`


        * `ElementStats._reduce_dimension()`


        * `ElementStats._sklearn_auto_wrap_output_keys`


        * `ElementStats.describer_type`


        * `ElementStats.from_data()`


        * `ElementStats.from_file()`


        * `ElementStats.transform_one()`


    * `M3GNetStructure`


        * `M3GNetStructure._abc_impl`


        * `M3GNetStructure._sklearn_auto_wrap_output_keys`


        * `M3GNetStructure.transform_one()`


    * `MEGNetSite`


        * `MEGNetSite._abc_impl`


        * `MEGNetSite._sklearn_auto_wrap_output_keys`


        * `MEGNetSite.describer_type`


        * `MEGNetSite.transform_one()`


    * `MEGNetStructure`


        * `MEGNetStructure._abc_impl`


        * `MEGNetStructure._sklearn_auto_wrap_output_keys`


        * `MEGNetStructure.describer_type`


        * `MEGNetStructure.transform_one()`


    * `RadialDistributionFunction`


        * `RadialDistributionFunction._get_specie_density()`


        * `RadialDistributionFunction.get_site_coordination()`


        * `RadialDistributionFunction.get_site_rdf()`


        * `RadialDistributionFunction.get_species_coordination()`


        * `RadialDistributionFunction.get_species_rdf()`


    * `RandomizedCoulombMatrix`


        * `RandomizedCoulombMatrix._abc_impl`


        * `RandomizedCoulombMatrix._sklearn_auto_wrap_output_keys`


        * `RandomizedCoulombMatrix.describer_type`


        * `RandomizedCoulombMatrix.get_randomized_coulomb_mat()`


        * `RandomizedCoulombMatrix.transform_one()`


    * `SiteElementProperty`


        * `SiteElementProperty._abc_impl`


        * `SiteElementProperty._get_keys()`


        * `SiteElementProperty._sklearn_auto_wrap_output_keys`


        * `SiteElementProperty.describer_type`


        * `SiteElementProperty.feature_dim`


        * `SiteElementProperty.transform_one()`


    * `SmoothOverlapAtomicPosition`


        * `SmoothOverlapAtomicPosition._abc_impl`


        * `SmoothOverlapAtomicPosition._sklearn_auto_wrap_output_keys`


        * `SmoothOverlapAtomicPosition.describer_type`


        * `SmoothOverlapAtomicPosition.transform_one()`


    * `SortedCoulombMatrix`


        * `SortedCoulombMatrix._abc_impl`


        * `SortedCoulombMatrix._sklearn_auto_wrap_output_keys`


        * `SortedCoulombMatrix.describer_type`


        * `SortedCoulombMatrix.get_sorted_coulomb_mat()`


        * `SortedCoulombMatrix.transform_one()`


    * `wrap_matminer_describer()`


    * maml.describers._composition module


        * `ElementStats`


            * `ElementStats.ALLOWED_STATS`


            * `ElementStats.AVAILABLE_DATA`


            * `ElementStats._abc_impl`


            * `ElementStats._reduce_dimension()`


            * `ElementStats._sklearn_auto_wrap_output_keys`


            * `ElementStats.describer_type`


            * `ElementStats.from_data()`


            * `ElementStats.from_file()`


            * `ElementStats.transform_one()`


        * `_is_element_or_specie()`


        * `_keys_are_elements()`


    * maml.describers._m3gnet module


        * `M3GNetStructure`


            * `M3GNetStructure._abc_impl`


            * `M3GNetStructure._sklearn_auto_wrap_output_keys`


            * `M3GNetStructure.transform_one()`


    * maml.describers._matminer module


        * `wrap_matminer_describer()`


    * maml.describers._megnet module


        * `MEGNetNotFound`


        * `MEGNetSite`


            * `MEGNetSite._abc_impl`


            * `MEGNetSite._sklearn_auto_wrap_output_keys`


            * `MEGNetSite.describer_type`


            * `MEGNetSite.transform_one()`


        * `MEGNetStructure`


            * `MEGNetStructure._abc_impl`


            * `MEGNetStructure._sklearn_auto_wrap_output_keys`


            * `MEGNetStructure.describer_type`


            * `MEGNetStructure.transform_one()`


        * `_load_model()`


    * maml.describers._rdf module


        * `RadialDistributionFunction`


            * `RadialDistributionFunction._get_specie_density()`


            * `RadialDistributionFunction.get_site_coordination()`


            * `RadialDistributionFunction.get_site_rdf()`


            * `RadialDistributionFunction.get_species_coordination()`


            * `RadialDistributionFunction.get_species_rdf()`


        * `_dist_to_counts()`


        * `get_pair_distances()`


    * maml.describers._site module


        * `BPSymmetryFunctions`


            * `BPSymmetryFunctions._abc_impl`


            * `BPSymmetryFunctions._fc()`


            * `BPSymmetryFunctions._sklearn_auto_wrap_output_keys`


            * `BPSymmetryFunctions.describer_type`


            * `BPSymmetryFunctions.transform_one()`


        * `BispectrumCoefficients`


            * `BispectrumCoefficients._abc_impl`


            * `BispectrumCoefficients._sklearn_auto_wrap_output_keys`


            * `BispectrumCoefficients.describer_type`


            * `BispectrumCoefficients.feature_dim`


            * `BispectrumCoefficients.subscripts`


            * `BispectrumCoefficients.transform_one()`


        * `MEGNetSite`


            * `MEGNetSite._abc_impl`


            * `MEGNetSite._sklearn_auto_wrap_output_keys`


            * `MEGNetSite.describer_type`


            * `MEGNetSite.transform_one()`


        * `SiteElementProperty`


            * `SiteElementProperty._abc_impl`


            * `SiteElementProperty._get_keys()`


            * `SiteElementProperty._sklearn_auto_wrap_output_keys`


            * `SiteElementProperty.describer_type`


            * `SiteElementProperty.feature_dim`


            * `SiteElementProperty.transform_one()`


        * `SmoothOverlapAtomicPosition`


            * `SmoothOverlapAtomicPosition._abc_impl`


            * `SmoothOverlapAtomicPosition._sklearn_auto_wrap_output_keys`


            * `SmoothOverlapAtomicPosition.describer_type`


            * `SmoothOverlapAtomicPosition.transform_one()`


    * maml.describers._spectrum module


    * maml.describers._structure module


        * `CoulombEigenSpectrum`


            * `CoulombEigenSpectrum._abc_impl`


            * `CoulombEigenSpectrum._sklearn_auto_wrap_output_keys`


            * `CoulombEigenSpectrum.describer_type`


            * `CoulombEigenSpectrum.transform_one()`


        * `CoulombMatrix`


            * `CoulombMatrix._abc_impl`


            * `CoulombMatrix._get_columb_mat()`


            * `CoulombMatrix._sklearn_auto_wrap_output_keys`


            * `CoulombMatrix.describer_type`


            * `CoulombMatrix.get_coulomb_mat()`


            * `CoulombMatrix.transform_one()`


        * `DistinctSiteProperty`


            * `DistinctSiteProperty._abc_impl`


            * `DistinctSiteProperty._sklearn_auto_wrap_output_keys`


            * `DistinctSiteProperty.describer_type`


            * `DistinctSiteProperty.supported_properties`


            * `DistinctSiteProperty.transform_one()`


        * `RandomizedCoulombMatrix`


            * `RandomizedCoulombMatrix._abc_impl`


            * `RandomizedCoulombMatrix._sklearn_auto_wrap_output_keys`


            * `RandomizedCoulombMatrix.describer_type`


            * `RandomizedCoulombMatrix.get_randomized_coulomb_mat()`


            * `RandomizedCoulombMatrix.transform_one()`


        * `SortedCoulombMatrix`


            * `SortedCoulombMatrix._abc_impl`


            * `SortedCoulombMatrix._sklearn_auto_wrap_output_keys`


            * `SortedCoulombMatrix.describer_type`


            * `SortedCoulombMatrix.get_sorted_coulomb_mat()`


            * `SortedCoulombMatrix.transform_one()`


* [maml.models package](maml.models.md)


    * `AtomSets`


        * `AtomSets._get_data_generator()`


        * `AtomSets._predict()`


        * `AtomSets.evaluate()`


        * `AtomSets.fit()`


        * `AtomSets.from_dir()`


        * `AtomSets.save()`


    * `KerasModel`


        * `KerasModel._get_validation_data()`


        * `KerasModel.fit()`


    * `MLP`


    * `SKLModel`


    * `WeightedAverageLayer`


        * `WeightedAverageLayer.build()`


        * `WeightedAverageLayer.call()`


        * `WeightedAverageLayer.compute_output_shape()`


        * `WeightedAverageLayer.get_config()`


        * `WeightedAverageLayer.reduce_sum()`


    * `WeightedSet2Set`


        * `WeightedSet2Set._lstm()`


        * `WeightedSet2Set.build()`


        * `WeightedSet2Set.call()`


        * `WeightedSet2Set.compute_output_shape()`


        * `WeightedSet2Set.get_config()`


    * Subpackages


        * [maml.models.dl package](maml.models.dl.md)


            * `AtomSets`


                * `AtomSets._get_data_generator()`


                * `AtomSets._predict()`


                * `AtomSets.evaluate()`


                * `AtomSets.fit()`


                * `AtomSets.from_dir()`


                * `AtomSets.save()`


            * `MLP`


            * `WeightedAverageLayer`


                * `WeightedAverageLayer.build()`


                * `WeightedAverageLayer.call()`


                * `WeightedAverageLayer.compute_output_shape()`


                * `WeightedAverageLayer.get_config()`


                * `WeightedAverageLayer.reduce_sum()`


            * `WeightedSet2Set`


                * `WeightedSet2Set._lstm()`


                * `WeightedSet2Set.build()`


                * `WeightedSet2Set.call()`


                * `WeightedSet2Set.compute_output_shape()`


                * `WeightedSet2Set.get_config()`


            * maml.models.dl._atomsets module


                * `AtomSets`


                    * `AtomSets._get_data_generator()`


                    * `AtomSets._predict()`


                    * `AtomSets.evaluate()`


                    * `AtomSets.fit()`


                    * `AtomSets.from_dir()`


                    * `AtomSets.save()`


                * `construct_atom_sets()`


            * maml.models.dl._keras_utils module


                * `deserialize_keras_activation()`


                * `deserialize_keras_optimizer()`


            * maml.models.dl._layers module


                * `WeightedAverageLayer`


                    * `WeightedAverageLayer.build()`


                    * `WeightedAverageLayer.call()`


                    * `WeightedAverageLayer.compute_output_shape()`


                    * `WeightedAverageLayer.get_config()`


                    * `WeightedAverageLayer.reduce_sum()`


                * `WeightedSet2Set`


                    * `WeightedSet2Set._lstm()`


                    * `WeightedSet2Set.build()`


                    * `WeightedSet2Set.call()`


                    * `WeightedSet2Set.compute_output_shape()`


                    * `WeightedSet2Set.get_config()`


            * maml.models.dl._mlp module


                * `MLP`


                * `construct_mlp()`


* [maml.sampling package](maml.sampling.md)


    * maml.sampling.clustering module


        * `BirchClustering`


            * `BirchClustering._sklearn_auto_wrap_output_keys`


            * `BirchClustering.fit()`


            * `BirchClustering.transform()`


    * maml.sampling.direct module


    * maml.sampling.pca module


        * `PrincipalComponentAnalysis`


            * `PrincipalComponentAnalysis._sklearn_auto_wrap_output_keys`


            * `PrincipalComponentAnalysis.fit()`


            * `PrincipalComponentAnalysis.transform()`


    * maml.sampling.stratified_sampling module


        * `SelectKFromClusters`


            * `SelectKFromClusters._sklearn_auto_wrap_output_keys`


            * `SelectKFromClusters.fit()`


            * `SelectKFromClusters.transform()`


* [maml.utils package](maml.utils.md)


    * `ConstantValue`


        * `ConstantValue.get_value()`


    * `DataSplitter`


        * `DataSplitter.split()`


    * `DummyScaler`


        * `DummyScaler.from_training_data()`


        * `DummyScaler.inverse_transform()`


        * `DummyScaler.transform()`


    * `LinearProfile`


        * `LinearProfile.get_value()`


    * `MultiScratchDir`


        * `MultiScratchDir.SCR_LINK`


    * `Scaler`


        * `Scaler.inverse_transform()`


        * `Scaler.transform()`


    * `ShuffleSplitter`


        * `ShuffleSplitter.split()`


    * `StandardScaler`


        * `StandardScaler.from_training_data()`


        * `StandardScaler.inverse_transform()`


        * `StandardScaler.transform()`


    * `Stats`


        * `Stats.allowed_stats`


        * `Stats.average()`


        * `Stats.geometric_mean()`


        * `Stats.harmonic_mean()`


        * `Stats.inverse_mean()`


        * `Stats.kurtosis()`


        * `Stats.max()`


        * `Stats.mean()`


        * `Stats.mean_absolute_deviation()`


        * `Stats.mean_absolute_error()`


        * `Stats.min()`


        * `Stats.mode()`


        * `Stats.moment()`


        * `Stats.power_mean()`


        * `Stats.range()`


        * `Stats.shifted_geometric_mean()`


        * `Stats.skewness()`


        * `Stats.std()`


    * `ValueProfile`


        * `ValueProfile.get_value()`


        * `ValueProfile.get_value()`


        * `ValueProfile.increment_step()`


    * `check_structures_forces_stresses()`


    * `convert_docs()`


    * `cwt()`


    * `feature_dim_from_test_system()`


    * `fft_magnitude()`


    * `get_describer_dummy_obj()`


    * `get_full_args()`


    * `get_full_stats_and_funcs()`


    * `get_lammps_lattice_and_rotation()`


    * `get_sp_method()`


    * `njit()`


    * `pool_from()`


    * `spectrogram()`


    * `stats_list_conversion()`


    * `stress_format_change()`


    * `stress_list_to_matrix()`


    * `stress_matrix_to_list()`


    * `to_array()`


    * `to_composition()`


    * `write_data_from_structure()`


    * `wvd()`


    * maml.utils._data_conversion module


        * `convert_docs()`


        * `doc_from()`


        * `pool_from()`


        * `to_array()`


    * maml.utils._data_split module


        * `DataSplitter`


            * `DataSplitter.split()`


        * `ShuffleSplitter`


            * `ShuffleSplitter.split()`


    * maml.utils._dummy module


        * `feature_dim_from_test_system()`


        * `get_describer_dummy_obj()`


    * maml.utils._inspect module


        * `get_full_args()`


        * `get_param_types()`


    * maml.utils._jit module


        * `njit()`


    * maml.utils._lammps module


        * `_get_atomic_mass()`


        * `_get_charge()`


        * `check_structures_forces_stresses()`


        * `get_lammps_lattice_and_rotation()`


        * `stress_format_change()`


        * `stress_list_to_matrix()`


        * `stress_matrix_to_list()`


        * `write_data_from_structure()`


    * maml.utils._material module


        * `to_composition()`


    * maml.utils._preprocessing module


        * `DummyScaler`


            * `DummyScaler.from_training_data()`


            * `DummyScaler.inverse_transform()`


            * `DummyScaler.transform()`


        * `Scaler`


            * `Scaler.inverse_transform()`


            * `Scaler.transform()`


        * `StandardScaler`


            * `StandardScaler.from_training_data()`


            * `StandardScaler.inverse_transform()`


            * `StandardScaler.transform()`


    * maml.utils._signal_processing module


        * `cwt()`


        * `fft_magnitude()`


        * `get_sp_method()`


        * `spectrogram()`


        * `wvd()`


    * maml.utils._stats module


        * `Stats`


            * `Stats.allowed_stats`


            * `Stats.average()`


            * `Stats.geometric_mean()`


            * `Stats.harmonic_mean()`


            * `Stats.inverse_mean()`


            * `Stats.kurtosis()`


            * `Stats.max()`


            * `Stats.mean()`


            * `Stats.mean_absolute_deviation()`


            * `Stats.mean_absolute_error()`


            * `Stats.min()`


            * `Stats.mode()`


            * `Stats.moment()`


            * `Stats.power_mean()`


            * `Stats.range()`


            * `Stats.shifted_geometric_mean()`


            * `Stats.skewness()`


            * `Stats.std()`


        * `_add_allowed_stats()`


        * `_convert_a_or_b()`


        * `_moment_symbol_conversion()`


        * `_root_moment()`


        * `get_full_stats_and_funcs()`


        * `stats_list_conversion()`


    * maml.utils._tempfile module


        * `MultiScratchDir`


            * `MultiScratchDir.SCR_LINK`


            * `MultiScratchDir.tempdirs`


        * `_copy_r_with_suffix()`


    * maml.utils._typing module


    * maml.utils._value_profile module


        * `ConstantValue`


            * `ConstantValue.get_value()`


        * `LinearProfile`


            * `LinearProfile.get_value()`


        * `ValueProfile`


            * `ValueProfile.get_value()`


            * `ValueProfile.get_value()`


            * `ValueProfile.increment_step()`
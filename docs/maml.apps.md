---
layout: default
title: maml.apps.md
nav_exclude: true
---

# maml.apps package

## Subpackages


* [maml.apps.bowsr package](maml.apps.bowsr.md)


    * Subpackages


        * [maml.apps.bowsr.model package](maml.apps.bowsr.model.md)


            * `EnergyModel`


                * `EnergyModel.predict_energy()`


            * maml.apps.bowsr.model.base module


                * `EnergyModel`


                    * `EnergyModel.predict_energy()`


            * maml.apps.bowsr.model.cgcnn module


            * maml.apps.bowsr.model.dft module


                * `DFT`


                    * `DFT.predict_energy()`


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
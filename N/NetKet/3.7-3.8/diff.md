# Comparing `tmp/netket-3.7.tar.gz` & `tmp/netket-3.8.tar.gz`

## Comparing `netket-3.7.tar` & `netket-3.8.tar`

### file list

```diff
@@ -1,242 +1,247 @@
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.7/netket/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 netket-3.7/netket/_version.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 netket-3.7/netket/exact.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.7/netket/callbacks/__init__.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 netket-3.7/netket/callbacks/earlystopping.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 netket-3.7/netket/callbacks/invalidlossstopping.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 netket-3.7/netket/callbacks/timeout.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 netket-3.7/netket/driver/__init__.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 netket-3.7/netket/driver/abstract_variational_driver.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 netket-3.7/netket/driver/steady_state.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 netket-3.7/netket/driver/vmc.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 netket-3.7/netket/driver/vmc_common.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/driver/__init__.py
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/driver/tdvp.py
--rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/driver/tdvp_common.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/driver/tdvp_schmitt.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/dynamics/__init__.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/dynamics/_rk_solver.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/dynamics/_rk_solver_structures.py
--rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/dynamics/_rk_tableau.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/hilbert/__init__.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/hilbert/spin_orbital_fermions.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/hilbert/random/__init__.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/hilbert/random/spin_orbital_fermions.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/logging/__init__.py
--rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/logging/hdf5_log.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/operator/__init__.py
--rw-r--r--   0        0        0    24940 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/operator/_fermion_operator_2nd.py
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/operator/_fermion_operator_2nd_utils.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/operator/fermion.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/qsr/__init__.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/qsr/dataset.py
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/qsr/driver.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/qsr/logic_helpers.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/sampler/__init__.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/sampler/metropolis_pmap.py
--rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/sampler/metropolis_pt.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/vqs/__init__.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 netket-3.7/netket/experimental/vqs/io.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/__init__.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/_lattice_edge_logic.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/abstract_graph.py
--rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/common_lattices.py
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/graph.py
--rw-r--r--   0        0        0    28276 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/lattice.py
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 netket-3.7/netket/graph/space_group.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/__init__.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/abstract_hilbert.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/continuous_hilbert.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/custom_hilbert.py
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/discrete_hilbert.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/doubled_hilbert.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/fock.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/hilbert_index.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/homogeneous.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/particle.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/qubit.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/spin.py
--rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/tensor_hilbert.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/__init__.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/base.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/custom.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/doubled.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/fock.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/particle.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/qubit.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/spin.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 netket-3.7/netket/hilbert/random/tensor_hilbert.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/__init__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_chunk_utils.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_expect.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_grad.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_math.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_scanmap.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_vjp.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_vjp_chunked.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_vmap_chunked.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/utils.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_jacobian/__init__.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_jacobian/jacobian_dense.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_jacobian/jacobian_pytree.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 netket-3.7/netket/jax/_jacobian/logic.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 netket-3.7/netket/logging/__init__.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 netket-3.7/netket/logging/json_log.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 netket-3.7/netket/logging/runtime_log.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 netket-3.7/netket/logging/state_log.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 netket-3.7/netket/logging/tensorboard.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 netket-3.7/netket/models/README.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 netket-3.7/netket/models/__init__.py
--rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 netket-3.7/netket/models/autoreg.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 netket-3.7/netket/models/deepset.py
--rw-r--r--   0        0        0    33655 2020-02-02 00:00:00.000000 netket-3.7/netket/models/equivariant.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 netket-3.7/netket/models/fast_autoreg.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 netket-3.7/netket/models/full_space.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 netket-3.7/netket/models/gaussian.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 netket-3.7/netket/models/jastrow.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 netket-3.7/netket/models/mlp.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 netket-3.7/netket/models/mps.py
--rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 netket-3.7/netket/models/ndm.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 netket-3.7/netket/models/rbm.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 netket-3.7/netket/models/utils.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/__init__.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/activation.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/deprecation.py
--rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/fast_masked_linear.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/initializers.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/masked_linear.py
--rw-r--r--   0        0        0    35492 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/symmetric_linear.py
--rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/utils.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/blocks/__init__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/blocks/deepset.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/blocks/mlp.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 netket-3.7/netket/nn/blocks/symmetry_sum.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/__init__.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_abstract_operator.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_abstract_super_operator.py
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_bose_hubbard.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_continuous_operator.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_discrete_operator.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_graph_operator.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_hamiltonian.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_heisenberg.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_ising.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_kinetic.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_lazy.py
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_local_liouvillian.py
--rw-r--r--   0        0        0    25078 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_local_operator.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_local_operator_compile_helpers.py
--rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_local_operator_helpers.py
--rw-r--r--   0        0        0    23208 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_pauli_strings.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_potential.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/_sumoperators.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/boson.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 netket-3.7/netket/operator/spin.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/__init__.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/linear_operator.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/preconditioner.py
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/sr.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/common.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/default.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/qgt_jacobian_common.py
--rw-r--r--   0        0        0    10366 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/qgt_jacobian_dense.py
--rw-r--r--   0        0        0    10939 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/qgt_jacobian_pytree.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/qgt_onthefly.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/qgt/qgt_onthefly_logic.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/solver/__init__.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.7/netket/optimizer/solver/solvers.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/__init__.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/autoreg.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/base.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/exact.py
--rw-r--r--   0        0        0    26652 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/metropolis.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/metropolis_numpy.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/__init__.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/base.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/continuous_gaussian.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/custom_numpy.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/exchange.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/hamiltonian.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/hamiltonian_numpy.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/langevin.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/local.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 netket-3.7/netket/sampler/rules/local_numpy.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 netket-3.7/netket/stats/__init__.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 netket-3.7/netket/stats/_autocorr.py
--rw-r--r--   0        0        0     9740 2020-02-02 00:00:00.000000 netket-3.7/netket/stats/mc_stats.py
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 netket-3.7/netket/stats/mc_stats_old.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 netket-3.7/netket/stats/mpi_stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netket-3.7/netket/tools/__init__.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 netket-3.7/netket/tools/_common.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 netket-3.7/netket/tools/_cpu_info.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 netket-3.7/netket/tools/_mpi_info.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 netket-3.7/netket/tools/check_mpi.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 netket-3.7/netket/tools/info.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/__init__.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/_dependencies_check.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/array.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/config_flags.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/deprecation.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/dispatch.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/errors.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/float.py
--rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/history.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/jax.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/moduletools.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/numbers.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/optional_deps.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/partial.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/seed.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/summation.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/types.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/version_check.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/__init__.py
--rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/_group.py
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/_permutation_group.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/_point_group.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/_semigroup.py
--rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/axial.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/cubic.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/icosa.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/group/planar.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/model_frameworks/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/model_frameworks/base.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/model_frameworks/flax.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/model_frameworks/haiku.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/model_frameworks/jax.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/mpi/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/mpi/mpi.py
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/mpi/primitives.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/struct/__init__.py
--rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/struct/dataclass.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 netket-3.7/netket/utils/struct/utils.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/__init__.py
--rw-r--r--   0        0        0    15628 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/base.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/experimental.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/exact/__init__.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/exact/expect.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/exact/state.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/common.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/kernels.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_mixed_state/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_mixed_state/expect.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_mixed_state/expect_chunked.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_mixed_state/state.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/__init__.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/expect.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/expect_chunked.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/expect_forces.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/expect_forces_chunked.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/expect_grad.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/expect_grad_chunked.py
--rw-r--r--   0        0        0    28563 2020-02-02 00:00:00.000000 netket-3.7/netket/vqs/mc/mc_state/state.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 netket-3.7/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 netket-3.7/LICENSE
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 netket-3.7/README.md
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 netket-3.7/pyproject.toml
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 netket-3.7/PKG-INFO
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.8/netket/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 netket-3.8/netket/_version.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 netket-3.8/netket/exact.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/__init__.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/earlystopping.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/invalidlossstopping.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/timeout.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/__init__.py
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/abstract_variational_driver.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/steady_state.py
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/vmc.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/vmc_common.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/__init__.py
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/tdvp.py
+-rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/tdvp_common.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/tdvp_schmitt.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/__init__.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/_rk_solver.py
+-rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/_rk_solver_structures.py
+-rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/_rk_tableau.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/__init__.py
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/spin_orbital_fermions.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/random/__init__.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/random/spin_orbital_fermions.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/logging/__init__.py
+-rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/logging/hdf5_log.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/__init__.py
+-rw-r--r--   0        0        0    24940 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/_fermion_operator_2nd.py
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/_fermion_operator_2nd_utils.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/fermion.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/__init__.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/dataset.py
+-rw-r--r--   0        0        0    19537 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/driver.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/logic_helpers.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/sampler/__init__.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/sampler/metropolis_pmap.py
+-rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/sampler/metropolis_pt.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/vqs/__init__.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/vqs/io.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/__init__.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/_lattice_edge_logic.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/abstract_graph.py
+-rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/common_lattices.py
+-rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/graph.py
+-rw-r--r--   0        0        0    28276 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/lattice.py
+-rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/space_group.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/__init__.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/abstract_hilbert.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/continuous_hilbert.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/custom_hilbert.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/discrete_hilbert.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/doubled_hilbert.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/fock.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/hilbert_index.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/homogeneous.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/particle.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/qubit.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/spin.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/tensor_hilbert.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/tensor_hilbert_discrete.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/__init__.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/base.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/custom.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/doubled.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/fock.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/particle.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/qubit.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/spin.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/tensor_hilbert.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_chunk_utils.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_expect.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_grad.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_math.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_scanmap.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_vjp.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_vjp_chunked.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_vmap_chunked.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/utils.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/__init__.py
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/default_mode.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/jacobian_dense.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/jacobian_pytree.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/logic.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/__init__.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/json_log.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/runtime_log.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/state_log.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/tensorboard.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 netket-3.8/netket/models/README.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 netket-3.8/netket/models/__init__.py
+-rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 netket-3.8/netket/models/autoreg.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 netket-3.8/netket/models/deepset.py
+-rw-r--r--   0        0        0    33655 2020-02-02 00:00:00.000000 netket-3.8/netket/models/equivariant.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 netket-3.8/netket/models/fast_autoreg.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 netket-3.8/netket/models/full_space.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 netket-3.8/netket/models/gaussian.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 netket-3.8/netket/models/jastrow.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 netket-3.8/netket/models/mlp.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 netket-3.8/netket/models/mps.py
+-rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 netket-3.8/netket/models/ndm.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 netket-3.8/netket/models/rbm.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 netket-3.8/netket/models/utils.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/__init__.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/activation.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/deprecation.py
+-rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/fast_masked_linear.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/initializers.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/masked_linear.py
+-rw-r--r--   0        0        0    35492 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/symmetric_linear.py
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/utils.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/__init__.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/deepset.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/mlp.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/symmetry_sum.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/__init__.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_abstract_operator.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_abstract_super_operator.py
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_bose_hubbard.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_continuous_operator.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_discrete_operator.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_graph_operator.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_hamiltonian.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_heisenberg.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_ising.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_kinetic.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_lazy.py
+-rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_liouvillian.py
+-rw-r--r--   0        0        0    25078 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_operator.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_operator_compile_helpers.py
+-rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_operator_helpers.py
+-rw-r--r--   0        0        0    23208 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_pauli_strings.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_potential.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_sumoperators.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/boson.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/spin.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/__init__.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/linear_operator.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/preconditioner.py
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/sr.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/common.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/default.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_common.py
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_dense.py
+-rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_onthefly.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_onthefly_logic.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/solver/__init__.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/solver/solvers.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/__init__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/autoreg.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/base.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/exact.py
+-rw-r--r--   0        0        0    26652 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/metropolis.py
+-rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/metropolis_numpy.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/__init__.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/base.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/continuous_gaussian.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/custom_numpy.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/exchange.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/fixed.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/hamiltonian.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/hamiltonian_numpy.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/langevin.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/local.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/local_numpy.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/multiple.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/tensor.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/__init__.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/_autocorr.py
+-rw-r--r--   0        0        0     9740 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/mc_stats.py
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/mc_stats_old.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/mpi_stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/__init__.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/_common.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/_cpu_info.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/_mpi_info.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/check_mpi.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/info.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/__init__.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/_dependencies_check.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/array.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/config_flags.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/deprecation.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/dispatch.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/errors.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/float.py
+-rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/history.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/jax.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/moduletools.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/numbers.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/optional_deps.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/partial.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/seed.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/summation.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/types.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/version_check.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/__init__.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_group.py
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_permutation_group.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_point_group.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_semigroup.py
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/axial.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/cubic.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/icosa.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/planar.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/base.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/flax.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/haiku.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/jax.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/mpi/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/mpi/mpi.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/mpi/primitives.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/struct/__init__.py
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/struct/dataclass.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/struct/utils.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/__init__.py
+-rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/base.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/experimental.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/exact/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/exact/expect.py
+-rw-r--r--   0        0        0    12301 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/exact/state.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/common.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/kernels.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/expect.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/expect_chunked.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py
+-rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/state.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/__init__.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_chunked.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_forces.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_forces_chunked.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_grad.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_grad_chunked.py
+-rw-r--r--   0        0        0    28665 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/state.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.8/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 netket-3.8/LICENSE
+-rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 netket-3.8/README.md
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 netket-3.8/pyproject.toml
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 netket-3.8/PKG-INFO
```

### Comparing `netket-3.7/netket/__init__.py` & `netket-3.8/netket/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/exact.py` & `netket-3.8/netket/exact.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/callbacks/__init__.py` & `netket-3.8/netket/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/callbacks/earlystopping.py` & `netket-3.8/netket/callbacks/earlystopping.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/callbacks/invalidlossstopping.py` & `netket-3.8/netket/callbacks/invalidlossstopping.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/callbacks/timeout.py` & `netket-3.8/netket/callbacks/timeout.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/driver/__init__.py` & `netket-3.8/netket/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/driver/abstract_variational_driver.py` & `netket-3.8/netket/driver/abstract_variational_driver.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/driver/steady_state.py` & `netket-3.8/netket/driver/steady_state.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/driver/vmc.py` & `netket-3.8/netket/driver/vmc.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/driver/vmc_common.py` & `netket-3.8/netket/driver/vmc_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/__init__.py` & `netket-3.8/netket/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/driver/__init__.py` & `netket-3.8/netket/experimental/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/driver/tdvp.py` & `netket-3.8/netket/experimental/driver/tdvp.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/driver/tdvp_common.py` & `netket-3.8/netket/experimental/driver/tdvp_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/driver/tdvp_schmitt.py` & `netket-3.8/netket/experimental/driver/tdvp_schmitt.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/dynamics/__init__.py` & `netket-3.8/netket/experimental/dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/dynamics/_rk_solver.py` & `netket-3.8/netket/experimental/dynamics/_rk_solver.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/dynamics/_rk_solver_structures.py` & `netket-3.8/netket/experimental/dynamics/_rk_solver_structures.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/dynamics/_rk_tableau.py` & `netket-3.8/netket/experimental/dynamics/_rk_tableau.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/hilbert/__init__.py` & `netket-3.8/netket/experimental/hilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/hilbert/spin_orbital_fermions.py` & `netket-3.8/netket/experimental/hilbert/spin_orbital_fermions.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from typing import Optional, List, Union
 from collections.abc import Iterable
 import numpy as np
 from fractions import Fraction
 
 from netket.hilbert.fock import Fock
-from netket.hilbert.tensor_hilbert import TensorHilbert
+from netket.hilbert.tensor_hilbert_discrete import TensorDiscreteHilbert
 from netket.hilbert.homogeneous import HomogeneousHilbert
 
 
 class SpinOrbitalFermions(HomogeneousHilbert):
     r"""
     Hilbert space for 2nd quantization fermions with spin `s` distributed among
     `n_orbital` orbitals.
@@ -88,15 +88,15 @@
             if len(n_fermions) != spin_size:
                 raise ValueError(
                     "list of number of fermions must equal number of spin components"
                 )
             spin_hilberts = [
                 Fock(n_max=1, N=n_orbitals, n_particles=Nf) for Nf in n_fermions
             ]
-            hilbert = TensorHilbert(*spin_hilberts)
+            hilbert = TensorDiscreteHilbert(*spin_hilberts)
 
         self._fock = hilbert
         """Internal representation of this Hilbert space (Fock or TensorHilbert)."""
         # local states are the occupation numbers (0, 1)
         local_states = np.array((0.0, 1.0))
 
         # we use the constraints from the Fock spaces, and override is_constrained later
```

### Comparing `netket-3.7/netket/experimental/hilbert/random/__init__.py` & `netket-3.8/netket/experimental/hilbert/random/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/hilbert/random/spin_orbital_fermions.py` & `netket-3.8/netket/experimental/hilbert/random/spin_orbital_fermions.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/logging/__init__.py` & `netket-3.8/netket/experimental/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/logging/hdf5_log.py` & `netket-3.8/netket/experimental/logging/hdf5_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/operator/__init__.py` & `netket-3.8/netket/experimental/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/operator/_fermion_operator_2nd.py` & `netket-3.8/netket/experimental/operator/_fermion_operator_2nd.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/operator/_fermion_operator_2nd_utils.py` & `netket-3.8/netket/experimental/operator/_fermion_operator_2nd_utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/operator/fermion.py` & `netket-3.8/netket/experimental/operator/fermion.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/qsr/__init__.py` & `netket-3.8/netket/experimental/qsr/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/qsr/dataset.py` & `netket-3.8/netket/experimental/qsr/dataset.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/qsr/driver.py` & `netket-3.8/netket/experimental/qsr/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
     def nll(self, return_stats: Optional[bool] = True):
         r"""
         Compute the Negative-Log-Likelihood over a batch of data.
 
         Args:
             return_stats: if True, return the statistics.
 
-        .. warn::
+        .. warning::
 
             Exponentially expensive in the hilbert space size!
 
         """
         log_val_rot = _local_value_rotated_amplitude(
             self.state._apply_fun,
             self.state.variables,
@@ -344,15 +344,15 @@
     def nll_whole_training_set(self, return_stats: Optional[bool] = True):
         r"""
         Compute the Negative-Log-Likelihood over the whole training set.
 
         Args:
             return_stats: if True, return the statistics.
 
-        .. warn::
+        .. warning::
 
             Exponentially expensive in the hilbert space size!
         """
         if self._chunk_size is not None:
             log_val_rot = []
             for i in range(self.n_chunk):
                 chunk_data = self.dataset[self._chunked_indices[i]]
@@ -408,15 +408,15 @@
         given by the target state in different measurement basis.
 
         Args:
             target_state: the target state.
             n_shots: number of shots per measurement basis.
             no_cache: if True, do not use the cached value.
 
-        .. warn::
+        .. warning::
 
             Exponentially expensive in the hilbert space size!
 
             Need to know the target state!
 
         """
         if len(target_state.shape) == 1:
@@ -440,15 +440,15 @@
         r"""
         Compute average KL divergence loss over a batch of data.
 
         Args:
             target_state: the target state.
             n_shots: number of shots per measurement basis.
 
-        .. warn::
+        .. warning::
 
             Exponentially expensive in the hilbert space size!
 
             Need to know the target state!
 
         """
         return statistics(
@@ -461,15 +461,15 @@
         r"""
         Compute average KL divergence loss over the whole training set.
 
         Args:
             target_state: the target state.
             n_shots: number of shots per measurement basis.
 
-        .. warn::
+        .. warning::
 
             Exponentially expensive in the hilbert space size!
 
             Need to know the target state!
 
         """
         return statistics(
@@ -483,15 +483,15 @@
         r"""
         Compute the average KL divergence loss between the variational state and the target state.
 
         Args:
             target_state: the target state.
             n_shots: number of shots per measurement basis.
 
-        .. warn::
+        .. warning::
 
             Exponentially expensive in the hilbert space size!
 
             Need to know the target state!
 
         """
         if len(target_state.shape) == 1:
```

### Comparing `netket-3.7/netket/experimental/qsr/logic_helpers.py` & `netket-3.8/netket/experimental/qsr/logic_helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/sampler/__init__.py` & `netket-3.8/netket/experimental/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/sampler/metropolis_pmap.py` & `netket-3.8/netket/experimental/sampler/metropolis_pmap.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/sampler/metropolis_pt.py` & `netket-3.8/netket/experimental/sampler/metropolis_pt.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/vqs/__init__.py` & `netket-3.8/netket/experimental/vqs/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/experimental/vqs/io.py` & `netket-3.8/netket/experimental/vqs/io.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/__init__.py` & `netket-3.8/netket/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/_lattice_edge_logic.py` & `netket-3.8/netket/graph/_lattice_edge_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/abstract_graph.py` & `netket-3.8/netket/graph/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/common_lattices.py` & `netket-3.8/netket/graph/common_lattices.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/graph.py` & `netket-3.8/netket/graph/graph.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/lattice.py` & `netket-3.8/netket/graph/lattice.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/graph/space_group.py` & `netket-3.8/netket/graph/space_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/__init__.py` & `netket-3.8/netket/hilbert/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 from .doubled_hilbert import DoubledHilbert
 from .spin import Spin
 from .fock import Fock
 from .qubit import Qubit
 from .particle import Particle
 
 from .tensor_hilbert import TensorHilbert
-
+from . import tensor_hilbert_discrete
 
 from netket.utils import _hide_submodules
 
 _hide_submodules(__name__)
```

### Comparing `netket-3.7/netket/hilbert/abstract_hilbert.py` & `netket-3.8/netket/hilbert/abstract_hilbert.py`

 * *Files 26% similar despite different names*

```diff
@@ -106,14 +106,53 @@
     @abc.abstractmethod
     def _attrs(self) -> Tuple:
         """
         Tuple of hashable attributes, used to compute the immutable
         hash of this Hilbert space
         """
 
+    def __mul__(self, other: "AbstractHilbert") -> "AbstractHilbert":
+        if not isinstance(other, AbstractHilbert):
+            return NotImplemented
+
+        if type(self) == type(other):
+            res = self._mul_sametype_(other)
+            if res is not NotImplemented:
+                return res
+
+        from .tensor_hilbert import TensorGenericHilbert
+
+        return TensorGenericHilbert(self, other)
+
+    def __rmul__(self, other: "AbstractHilbert") -> "AbstractHilbert":
+        if not isinstance(other, AbstractHilbert):
+            return NotImplemented
+
+        from .tensor_hilbert import TensorGenericHilbert
+
+        return TensorGenericHilbert(other, self)
+
+    def _mul_sametype_(self, other: "AbstractHilbert") -> "AbstractHilbert":
+        """This function can be implemented by subclasses to
+        specify how to multiply two Hilbert spaces of the same type.
+
+        This can be used as an optimization to avoid creating a TensorHilbert
+        object when possible, instead returning a new Hilbert space type.
+
+        If it is not possible to combine the two Hilbert spaces,
+        it should return NotImplemented.
+
+        Args:
+            other: other Hilbert space to combine with.
+
+        Returns:
+            An Hilbert space combining the two.
+        """
+        return NotImplemented
+
     def __eq__(self, other) -> bool:
         if isinstance(other, type(self)):
             return self._attrs == other._attrs
 
         return False
 
     def __hash__(self):
```

### Comparing `netket-3.7/netket/hilbert/continuous_hilbert.py` & `netket-3.8/netket/hilbert/continuous_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/custom_hilbert.py` & `netket-3.8/netket/hilbert/custom_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/discrete_hilbert.py` & `netket-3.8/netket/hilbert/discrete_hilbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import List, Tuple, Optional, Union, Iterator
 from textwrap import dedent
 from functools import reduce
 
 import numpy as np
 
 from netket.utils.types import Array
+from netket.utils.numbers import is_scalar
 
 from .abstract_hilbert import AbstractHilbert
 
 max_states = np.iinfo(np.int32).max
 """int: Maximum number of states that can be indexed"""
 
 
@@ -46,15 +47,15 @@
         """
         Initializes a discrete Hilbert space with a basis of given shape.
 
         Args:
             shape: The local dimension of the Hilbert space for each degree
                 of freedom.
         """
-        self._shape = shape
+        self._shape = tuple(shape)
 
         super().__init__()
 
     @property
     def shape(self) -> Tuple[int, ...]:
         r"""The size of the hilbert space on every site."""
         return self._shape
@@ -122,15 +123,15 @@
         """
         if out is None:
             out = np.empty((np.atleast_1d(numbers).shape[0], self.size))
 
         if np.any(numbers >= self.n_states):
             raise ValueError("numbers outside the range of allowed states")
 
-        if np.isscalar(numbers):
+        if is_scalar(numbers):
             return self._numbers_to_states(np.atleast_1d(numbers), out=out)[0, :]
         else:
             return self._numbers_to_states(numbers, out=out)
 
     def states_to_numbers(
         self, states: np.ndarray, out: Optional[np.ndarray] = None
     ) -> Union[int, np.ndarray]:
@@ -220,13 +221,20 @@
 
     def __mul__(self, other: "DiscreteHilbert"):
         if type(self) == type(other):
             res = self._mul_sametype_(other)
             if res is not NotImplemented:
                 return res
 
-        from .tensor_hilbert import TensorHilbert
+        if isinstance(other, DiscreteHilbert):
+            from .tensor_hilbert_discrete import TensorDiscreteHilbert
 
-        return TensorHilbert(self, other)
+            return TensorDiscreteHilbert(self, other)
+        elif isinstance(other, AbstractHilbert):
+            from .tensor_hilbert import TensorGenericHilbert
+
+            return TensorGenericHilbert(self, other)
+
+        return NotImplemented
 
     def __pow__(self, n):
         return reduce(lambda x, y: x * y, [self for _ in range(n)])
```

### Comparing `netket-3.7/netket/hilbert/doubled_hilbert.py` & `netket-3.8/netket/hilbert/doubled_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/fock.py` & `netket-3.8/netket/hilbert/fock.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/hilbert_index.py` & `netket-3.8/netket/hilbert/hilbert_index.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/homogeneous.py` & `netket-3.8/netket/hilbert/homogeneous.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         r"""Returns True if the hilbert space is constrained."""
         return self._constraint_fn is not None
 
     def _numbers_to_states(self, numbers: np.ndarray, out: np.ndarray) -> np.ndarray:
         if self.constrained:
             numbers = self._bare_numbers[numbers]
 
-        return self._hilbert_index.numbers_to_states(numbers, out)
+        return self._hilbert_index.numbers_to_states(np.asarray(numbers), out)
 
     def _states_to_numbers(self, states: np.ndarray, out: np.ndarray):
         self._hilbert_index.states_to_numbers(states, out)
 
         if self.constrained:
             out[:] = np.searchsorted(self._bare_numbers, out)
```

### Comparing `netket-3.7/netket/hilbert/particle.py` & `netket-3.8/netket/hilbert/particle.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/qubit.py` & `netket-3.8/netket/hilbert/qubit.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/spin.py` & `netket-3.8/netket/hilbert/spin.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/tensor_hilbert.py` & `netket-3.8/netket/hilbert/tensor_hilbert.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,194 +8,116 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Iterable, Tuple
+
+from abc import ABC
 
 import numpy as np
-import jax.numpy as jnp
 
-from .discrete_hilbert import DiscreteHilbert, _is_indexable
+from .abstract_hilbert import AbstractHilbert
+
 
+class TensorHilbert(ABC):
+    r"""Abstract base class for the tensor product of several sub-spaces,
+    representing the space.
 
-# TODO: Make parametric class
-class TensorHilbert(DiscreteHilbert):
-    r"""Tensor product of several Discrete sub-spaces, representing the space
+    This class can also be used to construct the correct type of TensorHilbert
+    subclass given the input types: if all input types are Generic hilbert spaces,
+    `TensorGeneralHilbert` will be constructed, while if they all are `DiscreteHilbert`
+    a `TensorDiscreteHilbert` will be created.
 
     In general you should not construct this object directly, but you should
     simply multiply different hilbert spaces together. In this case, Python's
     `*` operator will be interpreted as a tensor product.
 
-    This Hilbert can be used as a replacement anywhere a Uniform Hilbert space
-    is not required.
-
-    Examples:
-        Couple a bosonic mode with spins
+    This is an abstract mixing class that should be inherited from, together
+    with another class that inherits from `AbstractHilbert`.
+    """
 
-        >>> from netket.hilbert import Spin, Fock
-        >>> Fock(3)*Spin(0.5, 5)
-        Fock(n_max=3, N=1)⊗Spin(s=1/2, N=5)
-        >>> type(_)
-        <class 'netket.hilbert.tensor_hilbert.TensorHilbert'>
+    def __new__(cls, *args, **kwargs):
+        # This logic overrides the constructor, such that if someone tries to
+        # construct this class directly by calling `TensorHilbert(...)`
+        # it will construct either a DiscreteHilbert or TensorDiscreteHilbert
+        from .tensor_hilbert_discrete import TensorDiscreteHilbert, DiscreteHilbert
+
+        if cls is TensorHilbert:
+            if all(isinstance(hi, DiscreteHilbert) for hi in args):
+                cls = TensorDiscreteHilbert
+            else:
+                cls = TensorGenericHilbert
 
-    """
+        return super(TensorHilbert, cls).__new__(cls)
 
-    def __init__(self, *hilb_spaces: DiscreteHilbert):
-        r"""Constructs a tensor Hilbert space
+    def __init__(self, hilb_spaces: Iterable[AbstractHilbert], *args, **kwargs):
+        r"""Constructs a tensor Hilbert space.
 
         Args:
             *hilb: An iterable object containing at least 1 hilbert space.
         """
+        # Flatten "TensorHilberts" found inside hilb_spaces
+        _hilb_spaces_flat = []
+        for hi in hilb_spaces:
+            if isinstance(hi, TensorHilbert):
+                _hilb_spaces_flat.extend(hi.subspaces)
+            else:
+                _hilb_spaces_flat.append(hi)
+        hilb_spaces = _hilb_spaces_flat
 
-        self._hilbert_spaces = hilb_spaces
+        self._hilbert_spaces = tuple(hilb_spaces)
         self._n_hilbert_spaces = len(hilb_spaces)
         self._hilbert_i = np.concatenate(
             [[i for _ in range(hi.size)] for (i, hi) in enumerate(hilb_spaces)]
         )
 
         self._sizes = tuple([hi.size for hi in hilb_spaces])
-        shape = np.concatenate([hi.shape for hi in hilb_spaces])
         self._cum_sizes = np.cumsum(self._sizes)
         self._cum_indices = np.concatenate([[0], self._cum_sizes])
         self._size = sum(self._sizes)
         self._delta_indices_i = np.array(
             [self._cum_indices[i] for i in self._hilbert_i]
         )
-
-        # pre-compute indexing data iff the tensor space is still indexable
-        if all(hi.is_indexable for hi in hilb_spaces) and _is_indexable(shape):
-            self._ns_states = [hi.n_states for hi in self._hilbert_spaces]
-            self._ns_states_r = np.flip(self._ns_states)
-            self._cum_ns_states = np.concatenate([[0], np.cumprod(self._ns_states)])
-            self._cum_ns_states_r = np.flip(
-                np.cumprod(np.concatenate([[1], np.flip(self._ns_states)]))[:-1]
-            )
-            self._n_states = np.prod(self._ns_states)
-
-        super().__init__(shape=shape)
+        super().__init__(
+            *args, **kwargs
+        )  # forwards all unused arguments so that this class is a mixin.
 
     @property
     def size(self) -> int:
         return self._size
 
     @property
-    def is_finite(self):
-        return all([hi.is_finite for hi in self._hilbert_spaces])
+    def subspaces(self) -> Tuple[AbstractHilbert, ...]:
+        """Tuplec ontaining all the subspaces of this tensor product of
+        Hilbert spaces.
+        """
+        return self._hilbert_spaces
 
-    def _sub_index(self, i):
+    def _sub_index(self, i: int) -> int:
+        """Internal function computing the subspace index for the given site
+        i.
+
+        Arguments:
+            i: Index of a site in :math:`[0, N)`.
+        Returns:
+            The index `j` such that self.subspaces[j] is the Hilbert space
+            containing site `i`.
+        """
         for (j, sz) in enumerate(self._cum_sizes):
             if i < sz:
                 return j
 
-    # def size_at_index(self, i):
-    #    # j = self._sub_index(i)
-    #    # return self._hilbert_spaces[j].size_at_index(i-self._cum_indices[j-1])
-    #    return self._hilbert_spaces[self._hilbert_i[i]].size_at_index(
-    #        i - self._delta_indices_i[i]
-    #    )
-
-    def states_at_index(self, i):
-        # j = self._sub_index(i)
-        # return self._hilbert_spaces[j].states_at_index(i-self._cum_indices[j-1])
-        return self._hilbert_spaces[self._hilbert_i[i]].states_at_index(
-            i - self._delta_indices_i[i]
-        )
-
-    @property
-    def n_states(self) -> int:
-        if not self.is_indexable:
-            raise RuntimeError("The hilbert space is too large to be indexed.")
-        return self._n_states
-
-    def _numbers_to_states(self, numbers, out):
-        # !!! WARNING
-        # This code assumes that states are stored in a MSB
-        # (Most Significant Bit) format.
-        # We assume that the rightmost-half indexes the LSBs
-        # and the leftmost-half indexes the MSBs
-        # HilbertIndex-generated states respect this, as they are:
-        # 0 -> [0,0,0,0]
-        # 1 -> [0,0,0,1]
-        # 2 -> [0,0,1,0]
-        # etc...
-
-        rem = numbers
-        for (i, dim) in enumerate(self._ns_states_r):
-            rem, loc_numbers = np.divmod(rem, dim)
-            hi_i = self._n_hilbert_spaces - (i + 1)
-            self._hilbert_spaces[hi_i].numbers_to_states(
-                loc_numbers, out=out[:, self._cum_indices[hi_i] : self._cum_sizes[hi_i]]
-            )
-
-        return out
-
-    def _states_to_numbers(self, states, out):
-        out[:] = 0
-
-        temp = out.copy()
-
-        # !!! WARNING
-        # See note above in numbers_to_states
-
-        for (i, dim) in enumerate(self._cum_ns_states_r):
-            self._hilbert_spaces[i].states_to_numbers(
-                states[:, self._cum_indices[i] : self._cum_sizes[i]], out=temp
-            )
-            out += temp * dim
-
-        return out
-
-    def states_to_local_indices(self, x):
-        out = jnp.empty_like(x, dtype=jnp.int32)
-        for (i, hilb_i) in enumerate(self._hilbert_spaces):
-            out = out.at[..., self._cum_indices[i] : self._cum_sizes[i]].set(
-                hilb_i.states_to_local_indices(
-                    x[..., self._cum_indices[i] : self._cum_sizes[i]]
-                )
-            )
-        return out
-
-    def __repr__(self):
-        if len(self._hilbert_spaces) == 1:
-            return f"TensorHilbert({self._hilbert_spaces[0]})"
-
-        _str = "{}".format(self._hilbert_spaces[0])
-        for hi in self._hilbert_spaces[1:]:
-            _str += "⊗{}".format(hi)
-
-        return _str
-
     @property
     def _attrs(self):
         return self._hilbert_spaces
 
-    def __mul__(self, other):
-        spaces_l = self._hilbert_spaces[:-1]
-        space_center_l = self._hilbert_spaces[-1]
-
-        if isinstance(other, TensorHilbert):
-            space_center_r = other._hilbert_spaces[0]
-            spaces_r = other._hilbert_spaces[1:]
-        else:
-            space_center_r = other
-            spaces_r = tuple()
-
-        # Attempt to 'merge' the two spaces at the interface.
-        spaces_center = space_center_l * space_center_r
-        if isinstance(spaces_center, TensorHilbert):
-            spaces_center = (space_center_l, space_center_r)
-        else:
-            spaces_center = (spaces_center,)
-
-        return TensorHilbert(*spaces_l, *spaces_center, *spaces_r)
-
-    def ptrace(self, sites: Union[int, List]) -> Optional[DiscreteHilbert]:
+    def ptrace(self, sites: Union[int, List]) -> Optional[AbstractHilbert]:
         if isinstance(sites, int):
             sites = [sites]
 
         sites = np.sort(sites)
 
         for site in sites:
             if site < 0 or site >= self.size:
@@ -227,7 +149,48 @@
             elif len(new_hilberts) >= 1:
                 hilb = new_hilberts[0]
 
                 for h in new_hilberts[1:]:
                     hilb = hilb * h
 
                 return hilb
+
+    def __repr__(self):
+        if len(self._hilbert_spaces) == 1:
+            return f"{type(self).__name__}({self._hilbert_spaces[0]})"
+
+        _str = "{}".format(self._hilbert_spaces[0])
+        for hi in self._hilbert_spaces[1:]:
+            _str += "⊗{}".format(hi)
+
+        return _str
+
+
+class TensorGenericHilbert(TensorHilbert, AbstractHilbert):
+    def __init__(self, *hilb_spaces: AbstractHilbert):
+        if not all(isinstance(hi, AbstractHilbert) for hi in hilb_spaces):
+            raise TypeError(
+                "Arguments to TensorHilbert must all be subtypes of "
+                "AbstractHilbert. However the types are:\n\n"
+                f"{list(type(hi) for hi in hilb_spaces)}\n"
+            )
+        super().__init__(hilb_spaces)
+
+    def __mul__(self, other):
+        spaces_l = self._hilbert_spaces[:-1]
+        space_center_l = self._hilbert_spaces[-1]
+
+        if isinstance(other, TensorHilbert):
+            space_center_r = other._hilbert_spaces[0]
+            spaces_r = other._hilbert_spaces[1:]
+        else:
+            space_center_r = other
+            spaces_r = tuple()
+
+        # Attempt to 'merge' the two spaces at the interface.
+        spaces_center = space_center_l * space_center_r
+        if isinstance(spaces_center, TensorHilbert):
+            spaces_center = (space_center_l, space_center_r)
+        else:
+            spaces_center = (spaces_center,)
+
+        return TensorGenericHilbert(*spaces_l, *spaces_center, *spaces_r)
```

### Comparing `netket-3.7/netket/hilbert/random/__init__.py` & `netket-3.8/netket/hilbert/random/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/base.py` & `netket-3.8/netket/hilbert/random/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/custom.py` & `netket-3.8/netket/hilbert/random/custom.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/doubled.py` & `netket-3.8/netket/hilbert/random/doubled.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/fock.py` & `netket-3.8/netket/hilbert/random/fock.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/particle.py` & `netket-3.8/netket/hilbert/random/particle.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/qubit.py` & `netket-3.8/netket/hilbert/random/qubit.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/spin.py` & `netket-3.8/netket/hilbert/random/spin.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/hilbert/random/tensor_hilbert.py` & `netket-3.8/netket/hilbert/random/tensor_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/__init__.py` & `netket-3.8/netket/jax/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 from ._chunk_utils import chunk, unchunk
 from ._scanmap import scan_reduce, scan_append, scan_append_reduce, scanmap
 from ._vjp_chunked import vjp_chunked
 from ._vmap_chunked import apply_chunked, vmap_chunked
 
 from ._math import logsumexp_cplx
 
-from ._jacobian import jacobian
+from ._jacobian import jacobian, jacobian_default_mode
 
 from netket.utils import _hide_submodules
 
 _hide_submodules(__name__)
```

### Comparing `netket-3.7/netket/jax/_chunk_utils.py` & `netket-3.8/netket/jax/_chunk_utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_expect.py` & `netket-3.8/netket/jax/_expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_grad.py` & `netket-3.8/netket/jax/_grad.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_math.py` & `netket-3.8/netket/jax/_math.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_scanmap.py` & `netket-3.8/netket/jax/_scanmap.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_vjp.py` & `netket-3.8/netket/jax/_vjp.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Callable, Tuple, Any, Union
+from functools import partial
 
 import jax
 
 from jax import numpy as jnp
 from jax.tree_util import tree_map
 
 
@@ -25,14 +26,34 @@
 
 # _grad_CC, _RR and _RC are the chunked gradient functions for machines going
 # from R -> C, R->R and R->C. Ditto for vjp
 # Thee reason why R->C is more complicated is that it splits the calculation
 # into the real and complex part in order to be more efficient.
 
 
+def _cmplx(re, im, conj=False):
+    """
+    Safely convert real and imaginary part to a complex number, considering
+    `float0` dtypes which cannot be summed upon.
+
+    Those types appear when computing the `vjp` of functions with integer
+    inputs.
+    """
+    # detect tangent-0 dtypes
+    is_re_0 = jax.dtypes.issubdtype(re.dtype, jax.dtypes.float0)
+    is_im_0 = jax.dtypes.issubdtype(re.dtype, jax.dtypes.float0)
+    if is_re_0 or is_im_0:
+        return re
+    else:
+        if conj:
+            return re - 1j * im
+        else:
+            return re + 1j * im
+
+
 def vjp_cc(
     fun: Callable, *primals, has_aux: bool = False, conjugate: bool = False
 ) -> Union[Tuple[Any, Callable], Tuple[Any, Callable, Any]]:
     if has_aux:
         out, _vjp_fun, aux = jax.vjp(fun, *primals, has_aux=True)
     else:
         out, _vjp_fun = jax.vjp(fun, *primals, has_aux=False)
@@ -66,18 +87,15 @@
         function computing the vjp product for a R->R function.
         """
         if not jnp.iscomplexobj(ȳ):
             out = _vjp_fun(jnp.asarray(ȳ, dtype=primals_out.dtype))
         else:
             out_r = _vjp_fun(jnp.asarray(ȳ.real, dtype=primals_out.dtype))
             out_i = _vjp_fun(jnp.asarray(ȳ.imag, dtype=primals_out.dtype))
-            if conjugate:
-                out = tree_map(lambda re, im: re - 1j * im, out_r, out_i)
-            else:
-                out = tree_map(lambda re, im: re + 1j * im, out_r, out_i)
+            out = tree_map(partial(_cmplx, conj=conjugate), out_r, out_i)
 
         return out
 
     if has_aux:
         return primals_out, vjp_fun, aux
     else:
         return primals_out, vjp_fun
@@ -117,34 +135,30 @@
 
         # val = vals_r + vals_j
         vr_jr = vjp_r_fun(jnp.asarray(ȳ_r, dtype=vals_r.dtype))
         vj_jr = vjp_r_fun(jnp.asarray(ȳ_j, dtype=vals_r.dtype))
         vr_jj = vjp_j_fun(jnp.asarray(ȳ_r, dtype=vals_j.dtype))
         vj_jj = vjp_j_fun(jnp.asarray(ȳ_j, dtype=vals_j.dtype))
 
-        r = tree_map(
-            lambda re, im: re + 1j * im,
-            vr_jr,
-            vj_jr,
-        )
-        i = tree_map(lambda re, im: re + 1j * im, vr_jj, vj_jj)
-        out = tree_map(lambda re, im: re + 1j * im, r, i)
+        r = tree_map(_cmplx, vr_jr, vj_jr)
+        i = tree_map(_cmplx, vr_jj, vj_jj)
+        out = tree_map(_cmplx, r, i)
 
         if conjugate:
             out = tree_map(jnp.conjugate, out)
 
         return out
 
     if has_aux:
         return primals_out, vjp_fun, aux
     else:
         return primals_out, vjp_fun
 
 
-#  This function dispatches to the right
+# This function dispatches to the right
 def vjp(
     fun: Callable, *primals, has_aux: bool = False, conjugate: bool = False
 ) -> Union[Tuple[Any, Callable], Tuple[Any, Callable, Any]]:
 
     # output dtype
     out_shape = eval_shape(fun, *primals, has_aux=has_aux)
```

### Comparing `netket-3.7/netket/jax/_vjp_chunked.py` & `netket-3.8/netket/jax/_vjp_chunked.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,37 @@
     assert isinstance(t, tuple)
     if isinstance(nums, int):
         nums = (nums,)
     return tuple(r for i, r in enumerate(t) if i not in nums)
 
 
 def _vjp(fun, cotangents, *primals, nondiff_argnums=(), conjugate=False):
-    y, vjp_fun = nkvjp(fun, *primals, conjugate=conjugate)
+
+    # we pass a closure to vjp, capturing the nondiff_argnums
+    # this is necessary to avoid errors when using integer arguments
+    # resulting in float0 tangents, which nkvjp tries to conjugate, resulting in an error
+    # If we were to use the standard jax.vjp we could just trash the output at the end...
+
+    diff_args = tuple(a for i, a in enumerate(primals) if i not in nondiff_argnums)
+    nondiff_args = tuple(a for i, a in enumerate(primals) if i in nondiff_argnums)
+
+    def _fun(nondiff_argnums, nondiff_args, *diff_args):
+        n_args = len(nondiff_args) + len(diff_args)
+        it_nondiff = iter(nondiff_args)
+        it_diff = iter(diff_args)
+        args = tuple(
+            next(it_nondiff) if i in nondiff_argnums else next(it_diff)
+            for i in range(n_args)
+        )
+        return fun(*args)
+
+    y, vjp_fun = nkvjp(
+        partial(_fun, nondiff_argnums, nondiff_args), *diff_args, conjugate=conjugate
+    )
     res = vjp_fun(cotangents)
-    # trash non-needed tuple elements  of the output here
-    # since xla is probably not able to optimize it away through the scan/loop if its trashed at the end
-    # TODO pass closure to vjp instead ?
-    res = _trash_tuple_elements(res, nondiff_argnums)
     return (y,) + res
 
 
 def __vjp_fun_chunked(
     fun,
     primals,
     cotangents,
```

### Comparing `netket-3.7/netket/jax/_vmap_chunked.py` & `netket-3.8/netket/jax/_vmap_chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,69 +2,66 @@
 
 import jax
 import jax.numpy as jnp
 
 from ._chunk_utils import _chunk, _unchunk
 from ._scanmap import scanmap, scan_append
 
+from netket.utils import HashablePartial
+
+
+def _fun(vmapped_fun, chunk_size, argnums, *args, **kwargs):
+    n_elements = jax.tree_util.tree_leaves(args[argnums[0]])[0].shape[0]
+    n_chunks, n_rest = divmod(n_elements, chunk_size)
+
+    if n_chunks == 0 or chunk_size >= n_elements:
+        y = vmapped_fun(*args, **kwargs)
+    else:
+        # split inputs
+        def _get_chunks(x):
+            x_chunks = jax.tree_map(lambda x_: x_[: n_elements - n_rest, ...], x)
+            x_chunks = _chunk(x_chunks, chunk_size)
+            return x_chunks
+
+        def _get_rest(x):
+            x_rest = jax.tree_map(lambda x_: x_[n_elements - n_rest :, ...], x)
+            return x_rest
+
+        args_chunks = [
+            _get_chunks(a) if i in argnums else a for i, a in enumerate(args)
+        ]
+        args_rest = [_get_rest(a) if i in argnums else a for i, a in enumerate(args)]
+
+        y_chunks = _unchunk(
+            scanmap(vmapped_fun, scan_append, argnums)(*args_chunks, **kwargs)
+        )
+
+        if n_rest == 0:
+            y = y_chunks
+        else:
+            y_rest = vmapped_fun(*args_rest, **kwargs)
+            y = jax.tree_map(lambda y1, y2: jnp.concatenate((y1, y2)), y_chunks, y_rest)
+    return y
+
 
 def _chunk_vmapped_function(
     vmapped_fun: Callable, chunk_size: Optional[int], argnums=0
 ) -> Callable:
     """takes a vmapped function and computes it in chunks"""
 
     if chunk_size is None:
         return vmapped_fun
 
     if isinstance(argnums, int):
         argnums = (argnums,)
 
-    def _fun(*args, **kwargs):
-
-        n_elements = jax.tree_util.tree_leaves(args[argnums[0]])[0].shape[0]
-        n_chunks, n_rest = divmod(n_elements, chunk_size)
-
-        if n_chunks == 0 or chunk_size >= n_elements:
-            y = vmapped_fun(*args, **kwargs)
-        else:
-            # split inputs
-            def _get_chunks(x):
-                x_chunks = jax.tree_map(lambda x_: x_[: n_elements - n_rest, ...], x)
-                x_chunks = _chunk(x_chunks, chunk_size)
-                return x_chunks
-
-            def _get_rest(x):
-                x_rest = jax.tree_map(lambda x_: x_[n_elements - n_rest :, ...], x)
-                return x_rest
-
-            args_chunks = [
-                _get_chunks(a) if i in argnums else a for i, a in enumerate(args)
-            ]
-            args_rest = [
-                _get_rest(a) if i in argnums else a for i, a in enumerate(args)
-            ]
-
-            y_chunks = _unchunk(
-                scanmap(vmapped_fun, scan_append, argnums)(*args_chunks, **kwargs)
-            )
-
-            if n_rest == 0:
-                y = y_chunks
-            else:
-                y_rest = vmapped_fun(*args_rest, **kwargs)
-                y = jax.tree_map(
-                    lambda y1, y2: jnp.concatenate((y1, y2)), y_chunks, y_rest
-                )
-        return y
-
-    return _fun
+    return HashablePartial(_fun, vmapped_fun, chunk_size, argnums)
 
 
 def _parse_in_axes(in_axes):
-
     if isinstance(in_axes, int):
         in_axes = (in_axes,)
 
     if not set(in_axes).issubset((0, None)):
         raise NotImplementedError("Only in_axes 0/None are currently supported")
 
     argnums = tuple(
```

### Comparing `netket-3.7/netket/jax/utils.py` & `netket-3.8/netket/jax/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_jacobian/jacobian_dense.py` & `netket-3.8/netket/jax/_jacobian/jacobian_dense.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_jacobian/jacobian_pytree.py` & `netket-3.8/netket/jax/_jacobian/jacobian_pytree.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/jax/_jacobian/logic.py` & `netket-3.8/netket/jax/_jacobian/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     pdf: Array = None,
     chunk_size: int = None,
     center: bool = False,
     dense: bool = False,
 ) -> PyTree:
     r"""
     Computes the jacobian of a NN model with respect to its parameters. This function differs from
-    :ref:`jax.jac_bwd` because it supports models with both real and complex parameters, as well as
+    :ref:`jax.jacrev` because it supports models with both real and complex parameters, as well as
     non-holomorphic models.
 
     In the context of NQS, if you pass the log-wavefunction to to this function, it will compute the
     log-derivative of the wavefunction with respect to the parameters, i.e. the matrix commonly known
     as:
 
     .. math::
```

### Comparing `netket-3.7/netket/logging/__init__.py` & `netket-3.8/netket/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/logging/json_log.py` & `netket-3.8/netket/logging/json_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/logging/runtime_log.py` & `netket-3.8/netket/logging/runtime_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/logging/state_log.py` & `netket-3.8/netket/logging/state_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/logging/tensorboard.py` & `netket-3.8/netket/logging/tensorboard.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/__init__.py` & `netket-3.8/netket/models/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/autoreg.py` & `netket-3.8/netket/models/autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/deepset.py` & `netket-3.8/netket/models/deepset.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/equivariant.py` & `netket-3.8/netket/models/equivariant.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/fast_autoreg.py` & `netket-3.8/netket/models/fast_autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/full_space.py` & `netket-3.8/netket/models/full_space.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/gaussian.py` & `netket-3.8/netket/models/gaussian.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/jastrow.py` & `netket-3.8/netket/models/jastrow.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/mlp.py` & `netket-3.8/netket/models/mlp.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/mps.py` & `netket-3.8/netket/models/mps.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/ndm.py` & `netket-3.8/netket/models/ndm.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/rbm.py` & `netket-3.8/netket/models/rbm.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/models/utils.py` & `netket-3.8/netket/models/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/__init__.py` & `netket-3.8/netket/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/activation.py` & `netket-3.8/netket/nn/activation.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/deprecation.py` & `netket-3.8/netket/nn/deprecation.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/fast_masked_linear.py` & `netket-3.8/netket/nn/fast_masked_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/initializers.py` & `netket-3.8/netket/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/masked_linear.py` & `netket-3.8/netket/nn/masked_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/symmetric_linear.py` & `netket-3.8/netket/nn/symmetric_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/utils.py` & `netket-3.8/netket/nn/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from functools import partial, reduce
-from typing import Tuple, Optional
+from typing import Callable, Optional, Tuple
 import operator
 
 import jax
 from jax import numpy as jnp
 import numpy as np
 
+from netket import jax as nkjax
 from netket.utils import get_afun_if_module, mpi, module_version
-from netket.utils.types import Array
+from netket.utils.types import Array, PyTree
 from netket.hilbert import DiscreteHilbert
 
 from flax.traverse_util import flatten_dict, unflatten_dict
 from flax.core import unfreeze
 
 
-def split_array_mpi(array):
+def split_array_mpi(array: Array) -> Array:
     """
     Splits the first dimension of the input array among mpi processes.
     Works like `mpi.scatter`, but assumes that the input array is available and
     identical on all ranks.
     !!! Warn
          The output is a numpy array.
     Args:
@@ -47,22 +48,33 @@
 
     # divide the hilbert space in chunks for each node
     states_per_rank = np.array_split(states_n, mpi.n_nodes)
 
     return array[states_per_rank[mpi.rank]]
 
 
-def to_array(hilbert, apply_fun, variables, normalize=True, allgather=True):
+def to_array(
+    hilbert: DiscreteHilbert,
+    apply_fun: Callable[[PyTree, Array], Array],
+    variables: PyTree,
+    *,
+    normalize: bool = True,
+    allgather: bool = True,
+    chunk_size: Optional[int] = None,
+) -> Array:
     """
     Computes `apply_fun(variables, states)` on all states of `hilbert` and returns
       the results as a vector.
 
     Args:
         normalize: If True, the vector is normalized to have L2-norm 1.
         allgather: If True, the final wave function is stored in full at all MPI ranks.
+        chunk_size: Optional integer to specify the largest chunks of samples that
+            the model will be evaluated upon. By default it is `None`, and when specified
+            samples are split into chunks of at most `chunk_size`.
     """
     if not hilbert.is_indexable:
         raise RuntimeError("The hilbert space is not indexable")
 
     apply_fun = get_afun_if_module(apply_fun)
 
     # mpi4jax does not have (yet) allgatherv so we need to be creative
@@ -73,27 +85,37 @@
     fake_states_n = np.arange(n_states_padded - n_states)
 
     # divide the hilbert space in chunks for each node
     states_per_rank = np.split(np.concatenate([states_n, fake_states_n]), mpi.n_nodes)
 
     xs = hilbert.numbers_to_states(states_per_rank[mpi.rank])
 
-    return _to_array_rank(apply_fun, variables, xs, n_states, normalize, allgather)
+    return _to_array_rank(
+        apply_fun, variables, xs, n_states, normalize, allgather, chunk_size
+    )
 
 
-@partial(jax.jit, static_argnums=(0, 3, 4, 5))
-def _to_array_rank(apply_fun, variables, σ_rank, n_states, normalize, allgather):
+@partial(jax.jit, static_argnums=(0, 3, 4, 5, 6))
+def _to_array_rank(
+    apply_fun, variables, σ_rank, n_states, normalize, allgather, chunk_size
+):
     """
     Computes apply_fun(variables, σ_rank) and gathers all results across all ranks.
     The input σ_rank should be a slice of all states in the hilbert space of equal
     length across all ranks because mpi4jax does not support allgatherv (yet).
 
     Args:
         n_states: total number of elements in the hilbert space.
     """
+
+    if chunk_size is not None:
+        apply_fun = nkjax.apply_chunked(
+            apply_fun, in_axes=(None, 0), chunk_size=chunk_size
+        )
+
     # number of 'fake' states, in the last rank.
     n_fake_states = σ_rank.shape[0] * mpi.n_nodes - n_states
 
     log_psi_local = apply_fun(variables, σ_rank)
 
     # last rank, get rid of fake elements
     if mpi.rank == mpi.n_nodes - 1 and n_fake_states > 0:
@@ -120,20 +142,27 @@
     psi = psi.reshape(-1)
 
     # remove fake states
     psi = psi[0:n_states]
     return psi
 
 
-def to_matrix(hilbert, machine, params, normalize=True):
+def to_matrix(
+    hilbert: DiscreteHilbert,
+    machine: Callable[[PyTree, Array], Array],
+    params: PyTree,
+    *,
+    normalize: bool = True,
+    chunk_size: Optional[int] = None,
+) -> Array:
 
     if not hilbert.is_indexable:
         raise RuntimeError("The hilbert space is not indexable")
 
-    psi = to_array(hilbert, machine, params, normalize=False)
+    psi = to_array(hilbert, machine, params, normalize=False, chunk_size=chunk_size)
 
     L = hilbert.physical.n_states
     rho = psi.reshape((L, L))
     if normalize:
         trace = jnp.trace(rho)
         rho /= trace
```

### Comparing `netket-3.7/netket/nn/blocks/__init__.py` & `netket-3.8/netket/nn/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/blocks/deepset.py` & `netket-3.8/netket/nn/blocks/deepset.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/blocks/mlp.py` & `netket-3.8/netket/nn/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/nn/blocks/symmetry_sum.py` & `netket-3.8/netket/nn/blocks/symmetry_sum.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/__init__.py` & `netket-3.8/netket/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_abstract_operator.py` & `netket-3.8/netket/operator/_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_abstract_super_operator.py` & `netket-3.8/netket/operator/_abstract_super_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_bose_hubbard.py` & `netket-3.8/netket/operator/_bose_hubbard.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         assert isinstance(hilbert, Fock)
         super().__init__(hilbert)
 
         if dtype is None:
             dtype = jnp.promote_types(_dtype(U), _dtype(V))
             dtype = jnp.promote_types(dtype, _dtype(J))
             dtype = jnp.promote_types(dtype, _dtype(mu))
+        dtype = jnp.promote_types(float, dtype)
         dtype = np.empty((), dtype=dtype).dtype
         self._dtype = dtype
 
         self._U = np.asarray(U, dtype=dtype)
         self._V = np.asarray(V, dtype=dtype)
         self._J = np.asarray(J, dtype=dtype)
         self._mu = np.asarray(mu, dtype=dtype)
```

### Comparing `netket-3.7/netket/operator/_continuous_operator.py` & `netket-3.8/netket/operator/_continuous_operator.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import abc
-from typing import Optional, Callable
+from typing import Callable, Hashable, Optional, Tuple
 
 from netket.utils.types import DType, PyTree, Array
 
 from netket.hilbert import AbstractHilbert
 from netket.operator import AbstractOperator
 
 
@@ -34,14 +34,15 @@
 
         Args:
             hilbert: The underlying Hilbert space on which the operator is defined
             dtype: Data type of the matrix elements. Defaults to `np.float64`
         """
 
         self._dtype = dtype
+        self._hash = None
         super().__init__(hilbert)
 
     @property
     def dtype(self) -> DType:
         return self._dtype
 
     @abc.abstractmethod
@@ -68,14 +69,22 @@
         r"""This methods should return a PyTree that will be passed as the `data` argument
         to the `_expect_kernel`. The PyTree should be composed of jax arrays or hashable
         objects.
 
         For example for the kinetic energy this method would return the masses of the
         individual particles."""
 
+    @abc.abstractproperty
+    def _attrs(self) -> Tuple[Hashable, ...]:
+        """This must return a tuple of (hashable) attributes used to compare two operators of
+        the same type and that is hashed to compute the hash of the operator.
+
+        To hash arrays you can return them as `nk.utils.HashableArray`.
+        """
+
     def __add__(self, other):
         if isinstance(self, ContinuousOperator) and isinstance(
             other, ContinuousOperator
         ):
             from netket.operator import SumOperator
 
             return SumOperator(self, other)
@@ -100,7 +109,17 @@
         if isinstance(other, ContinuousOperator):
             return self + (-other)
         else:
             return NotImplemented  # pragma: no cover
 
     def __neg__(self):
         return -1.0 * self
+
+    def __hash__(self):
+        if self._hash is None:
+            self._hash = hash((type(self), self._attrs))
+        return self._hash
+
+    def __eq__(self, other) -> bool:
+        if isinstance(other, type(self)):
+            return self._attrs == other._attrs
+        return False
```

### Comparing `netket-3.7/netket/operator/_discrete_operator.py` & `netket-3.8/netket/operator/_discrete_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,20 +74,20 @@
         other quantum numbers  :math:`x'` such that the matrix element
         :math:`O(x,x')` is different from zero. In general there will be
         several different connected states :math:`x'` satisfying this
         condition, and they are denoted here :math:`x'(k)`, for
         :math:`k=0,1...N_{\mathrm{connected}}`.
 
         This is a batched version, where x is a matrix of shape
-        :math:`(batch_size,hilbert.size)`.
+        :code:`(batch_size,hilbert.size)`.
 
         Args:
-            x (matrix): A matrix of shape (batch_size,hilbert.size)
+            x: A matrix of shape `(batch_size, hilbert.size)`
                 containing the batch of quantum numbers x.
-            sections (array): An array of sections for the flattened x'.
+            sections: An array of sections for the flattened x'.
                 See numpy.split for the meaning of sections.
 
         Returns:
             (matrix, array): The connected states x', flattened together in
                 a single matrix.
                 An array containing the matrix elements :math:`O(x,x')`
                 associated to each x'.
@@ -96,19 +96,22 @@
 
     def get_conn(self, x: np.ndarray):
         r"""Finds the connected elements of the Operator. Starting
         from a given quantum number x, it finds all other quantum numbers x' such
         that the matrix element :math:`O(x,x')` is different from zero. In general there
         will be several different connected states x' satisfying this
         condition, and they are denoted here :math:`x'(k)`, for :math:`k=0,1...N_{\mathrm{connected}}`.
+
         Args:
-            x (array): An array of shape (hilbert.size) containing the quantum numbers x.
+            x: An array of shape `(hilbert.size, )` containing the quantum numbers x.
+
         Returns:
             matrix: The connected states x' of shape (N_connected,hilbert.size)
             array: An array containing the matrix elements :math:`O(x,x')` associated to each x'.
+
         Raise:
             ValueError: If the given quantum number is not compatible with the hilbert space.
         """
         if x.ndim != 1:
             raise ValueError(
                 "get_conn does not support batches. Please use get_conn_flattened instead."
             )
```

### Comparing `netket-3.7/netket/operator/_graph_operator.py` & `netket-3.8/netket/operator/_graph_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_hamiltonian.py` & `netket-3.8/netket/operator/_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_heisenberg.py` & `netket-3.8/netket/operator/_heisenberg.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_ising.py` & `netket-3.8/netket/operator/_ising.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_kinetic.py` & `netket-3.8/netket/operator/_kinetic.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,34 +19,35 @@
 import jax
 import jax.numpy as jnp
 
 from netket.utils.types import DType, PyTree, Array
 import netket.jax as nkjax
 from netket.hilbert import AbstractHilbert
 from netket.operator import ContinuousOperator
+from netket.utils import HashableArray
 
 
 def jacrev(f):
     def jacfun(x):
         y, vjp_fun = nkjax.vjp(f, x)
         if y.size == 1:
-            eye = jnp.eye(y.size)[0]
+            eye = jnp.eye(y.size, dtype=x.dtype)[0]
             J = jax.vmap(vjp_fun, in_axes=0)(eye)
         else:
-            eye = jnp.eye(y.size)
+            eye = jnp.eye(y.size, dtype=x.dtype)
             J = jax.vmap(vjp_fun, in_axes=0)(eye)
         return J
 
     return jacfun
 
 
 def jacfwd(f):
     def jacfun(x):
         jvp_fun = lambda s: jax.jvp(f, (x,), (s,))[1]
-        eye = jnp.eye(len(x))
+        eye = jnp.eye(len(x), dtype=x.dtype)
         J = jax.vmap(jvp_fun, in_axes=0)(eye)
         return J
 
     return jacfun
 
 
 class KineticEnergy(ContinuousOperator):
@@ -65,14 +66,15 @@
         mass: float if all masses are the same, list indicating the mass of each particle otherwise
         dtype: Data type of the matrix elements. Defaults to `np.float64`
         """
 
         self._mass = jnp.asarray(mass, dtype=dtype)
 
         self._is_hermitian = np.allclose(self._mass.imag, 0.0)
+        self.__attrs = None
 
         super().__init__(hilbert, self._mass.dtype)
 
     @property
     def mass(self):
         return self._mass
 
@@ -98,9 +100,15 @@
         self, logpsi: Callable, params: PyTree, x: Array, coefficient: Optional[PyTree]
     ):
         return self._expect_kernel_single(logpsi, params, x, coefficient)
 
     def _pack_arguments(self) -> PyTree:
         return 1.0 / self._mass
 
+    @property
+    def _attrs(self):
+        if self.__attrs is None:
+            self.__attrs = (self.hilbert, self.dtype, HashableArray(self.mass))
+        return self.__attrs
+
     def __repr__(self):
         return f"KineticEnergy(m={self._mass})"
```

### Comparing `netket-3.7/netket/operator/_lazy.py` & `netket-3.8/netket/operator/_lazy.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_local_liouvillian.py` & `netket-3.8/netket/operator/_local_liouvillian.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_local_operator.py` & `netket-3.8/netket/operator/_local_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_local_operator_compile_helpers.py` & `netket-3.8/netket/operator/_local_operator_compile_helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_local_operator_helpers.py` & `netket-3.8/netket/operator/_local_operator_helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_pauli_strings.py` & `netket-3.8/netket/operator/_pauli_strings.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/_potential.py` & `netket-3.8/netket/operator/_potential.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,44 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Optional, Callable
-from functools import partial
+from typing import Callable, Hashable, Optional, Tuple
 
 from netket.utils.types import DType, PyTree, Array
 
 from netket.hilbert import AbstractHilbert
 from netket.operator import ContinuousOperator
+from netket.utils import struct, HashableArray
 
 import jax
 import jax.numpy as jnp
 
 
+@struct.dataclass
+class PotentialOperatorPyTree:
+    """Internal class used to pass data from the operator to the jax kernel.
+
+    This is used such that we can pass a PyTree containing some static data.
+    We could avoid this if the operator itself was a pytree, but as this is not
+    the case we need to pass as a separte object all fields that are used in
+    the kernel.
+
+    We could forego this, but then the kernel could not be marked as
+    @staticmethod and we would recompile every time we construct a new operator,
+    even if it is identical
+    """
+
+    potential_fun: Callable = struct.field(pytree_node=False)
+    coefficient: Array
+
+
 class PotentialEnergy(ContinuousOperator):
     r"""Returns the local potential energy defined in afun"""
 
     def __init__(
         self,
         hilbert: AbstractHilbert,
         afun: Callable,
@@ -38,32 +56,43 @@
             hilbert: The underlying Hilbert space on which the operator is defined
             afun: The potential energy as function of x
             coefficients: A coefficient for the ContinuousOperator object
             dtype: Data type of the matrix elements. Defaults to `np.float64`
         """
 
         self._afun = afun
+        self._coefficient = jnp.array(coefficient, dtype=dtype)
 
-        self.coefficient = jnp.array(coefficient, dtype=dtype)
+        self.__attrs = None
 
         super().__init__(hilbert, self.coefficient.dtype)
 
-    def _expect_kernel_single(
-        self, logpsi: Callable, params: PyTree, x: Array, coefficient: Optional[PyTree]
-    ):
-        return coefficient * self._afun(x)
-
-    @partial(jax.vmap, in_axes=(None, None, None, 0, None))
-    def _expect_kernel(
-        self, logpsi: Callable, params: PyTree, x: Array, coefficient: Optional[PyTree]
-    ):
-        return self._expect_kernel_single(logpsi, params, x, coefficient)
+    @property
+    def coefficient(self) -> Array:
+        return self._coefficient
 
     @property
-    def is_hermitian(self):
+    def is_hermitian(self) -> bool:
         return True
 
-    def _pack_arguments(self):
-        return self.coefficient
+    @staticmethod
+    def _expect_kernel(
+        logpsi: Callable, params: PyTree, x: Array, data: Optional[PyTree]
+    ) -> Array:
+        return data.coefficient * jax.vmap(data.potential_fun, in_axes=(0,))(x)
+
+    def _pack_arguments(self) -> PotentialOperatorPyTree:
+        return PotentialOperatorPyTree(self._afun, self.coefficient)
+
+    @property
+    def _attrs(self) -> Tuple[Hashable, ...]:
+        if self.__attrs is None:
+            self.__attrs = (
+                self.hilbert,
+                self._afun,
+                self.dtype,
+                HashableArray(self.coefficient),
+            )
+        return self.__attrs
 
     def __repr__(self):
         return f"Potential(coefficient={self.coefficient}, function={self._afun})"
```

### Comparing `netket-3.7/netket/operator/boson.py` & `netket-3.8/netket/operator/boson.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/operator/spin.py` & `netket-3.8/netket/operator/spin.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/__init__.py` & `netket-3.8/netket/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/linear_operator.py` & `netket-3.8/netket/optimizer/linear_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/preconditioner.py` & `netket-3.8/netket/optimizer/preconditioner.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/sr.py` & `netket-3.8/netket/optimizer/sr.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/qgt/__init__.py` & `netket-3.8/netket/optimizer/qgt/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/qgt/common.py` & `netket-3.8/netket/optimizer/qgt/common.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/qgt/default.py` & `netket-3.8/netket/optimizer/qgt/default.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/qgt/qgt_jacobian_dense.py` & `netket-3.8/netket/optimizer/qgt/qgt_jacobian_dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import netket.jax as nkjax
 from netket.nn import split_array_mpi
 
 from ..linear_operator import LinearOperator, Uninitialized
 
 from .common import check_valid_vector_type
 from .qgt_jacobian_common import (
-    choose_jacobian_mode,
     sanitize_diag_shift,
     to_shift_offset,
     rescale,
 )
 
 
 def QGTJacobianDense(
@@ -108,15 +107,15 @@
         samples = split_array_mpi(vstate._all_states)
         pdf = split_array_mpi(vstate.probability_distribution())
     else:
         samples = vstate.samples
         pdf = None
 
     if mode is None:
-        mode = choose_jacobian_mode(
+        mode = nkjax.jacobian_default_mode(
             vstate._apply_fun,
             vstate.parameters,
             vstate.model_state,
             samples,
             holomorphic=holomorphic,
         )
```

### Comparing `netket-3.7/netket/optimizer/qgt/qgt_jacobian_pytree.py` & `netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from netket.nn import split_array_mpi
 
 from ..linear_operator import LinearOperator, Uninitialized
 
 from .common import check_valid_vector_type
 from .qgt_jacobian_pytree_logic import mat_vec
 from .qgt_jacobian_common import (
-    choose_jacobian_mode,
     sanitize_diag_shift,
     to_shift_offset,
     rescale,
 )
 
 
 def QGTJacobianPyTree(
@@ -110,15 +109,15 @@
         pdf = split_array_mpi(vstate.probability_distribution())
     else:
         samples = vstate.samples
         pdf = None
 
     # Choose sensible default mode
     if mode is None:
-        mode = choose_jacobian_mode(
+        mode = nkjax.jacobian_default_mode(
             vstate._apply_fun,
             vstate.parameters,
             vstate.model_state,
             samples,
             holomorphic=holomorphic,
         )
```

### Comparing `netket-3.7/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py` & `netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/qgt/qgt_onthefly.py` & `netket-3.8/netket/optimizer/qgt/qgt_onthefly.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/qgt/qgt_onthefly_logic.py` & `netket-3.8/netket/optimizer/qgt/qgt_onthefly_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/optimizer/solver/solvers.py` & `netket-3.8/netket/optimizer/solver/solvers.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/__init__.py` & `netket-3.8/netket/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/autoreg.py` & `netket-3.8/netket/sampler/autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/base.py` & `netket-3.8/netket/sampler/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/exact.py` & `netket-3.8/netket/sampler/exact.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/metropolis.py` & `netket-3.8/netket/sampler/metropolis.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/metropolis_numpy.py` & `netket-3.8/netket/sampler/metropolis_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/__init__.py` & `netket-3.8/netket/sampler/rules/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .base import MetropolisRule
 
+from .fixed import FixedRule
 from .local import LocalRule
 from .exchange import ExchangeRule
 from .hamiltonian import HamiltonianRule
 from .continuous_gaussian import GaussianRule
 from .langevin import LangevinRule
+from .tensor import tensorRule as TensorRule
+from .multiple import multipleRules as MultipleRules
 
 # numpy backend
 from .local_numpy import LocalRuleNumpy
 from .hamiltonian_numpy import HamiltonianRuleNumpy
 from .custom_numpy import CustomRuleNumpy
 
 from netket.utils import _hide_submodules
```

### Comparing `netket-3.7/netket/sampler/rules/base.py` & `netket-3.8/netket/sampler/rules/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/continuous_gaussian.py` & `netket-3.8/netket/sampler/rules/continuous_gaussian.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/custom_numpy.py` & `netket-3.8/netket/sampler/rules/custom_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/exchange.py` & `netket-3.8/netket/sampler/rules/exchange.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/hamiltonian.py` & `netket-3.8/netket/sampler/rules/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/hamiltonian_numpy.py` & `netket-3.8/netket/sampler/rules/hamiltonian_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/langevin.py` & `netket-3.8/netket/sampler/rules/langevin.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     [1]: https://en.wikipedia.org/wiki/Metropolis-adjusted_Langevin_algorithm
     """
 
     dt: float = 0.001
     """
     Time step in the Langevin dynamics
     """
-    chunk_size: int = None
+    chunk_size: int = struct.field(pytree_node=False, default=None)
     """
     Chunk size for computing gradients of the ansatz
     """
 
     def transition(rule, sampler, machine, parameters, state, key, r):
         if jnp.issubdtype(r.dtype, jnp.complexfloating):
             raise TypeError("LangevinRule does not work with complex basis elements.")
@@ -85,15 +85,16 @@
 
     def _log_prob(x):
         """Conversion to a log probability"""
         return machine_pow * apply_fun(parameters, x).real
 
     def _single_grad(x):
         """Derivative of log_prob with respect to a single sample x"""
-        g = nkjax.grad(_log_prob)(x)
+        x = x.reshape(x.shape[-1])
+        g = nkjax.grad(lambda xi: _log_prob(xi).ravel()[0])(x)
         return g if jnp.iscomplexobj(r) else g.real
 
     grad_logp_r = nkjax.vmap_chunked(_single_grad, chunk_size=chunk_size)(r)
 
     rp = r + dt * grad_logp_r + jnp.sqrt(2 * dt) * noise_vec
 
     if not return_log_corr:
```

### Comparing `netket-3.7/netket/sampler/rules/local.py` & `netket-3.8/netket/sampler/rules/local.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/sampler/rules/local_numpy.py` & `netket-3.8/netket/sampler/rules/local_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/stats/__init__.py` & `netket-3.8/netket/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/stats/_autocorr.py` & `netket-3.8/netket/stats/_autocorr.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/stats/mc_stats.py` & `netket-3.8/netket/stats/mc_stats.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/stats/mc_stats_old.py` & `netket-3.8/netket/stats/mc_stats_old.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/stats/mpi_stats.py` & `netket-3.8/netket/stats/mpi_stats.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/tools/_common.py` & `netket-3.8/netket/tools/_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/tools/_cpu_info.py` & `netket-3.8/netket/tools/_cpu_info.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/tools/_mpi_info.py` & `netket-3.8/netket/tools/_mpi_info.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/tools/check_mpi.py` & `netket-3.8/netket/tools/check_mpi.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/tools/info.py` & `netket-3.8/netket/tools/info.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/__init__.py` & `netket-3.8/netket/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .config_flags import config
 
+from .moduletools import _hide_submodules, rename_class, auto_export as _auto_export
+from .version_check import module_version
+
+# error if old dependencies are detected
+from . import _dependencies_check
+
 from . import dispatch
 from . import struct
 from . import numbers
 from . import types
 from . import float
 from . import errors
 
@@ -31,24 +37,19 @@
 from .deprecation import (
     warn_deprecation,
     deprecated,
     deprecated_new_name,
     deprecate_dtype,
     pure_callback,
 )
-from .moduletools import _hide_submodules, rename_class, auto_export as _auto_export
-from .version_check import module_version
 
 from .model_frameworks import maybe_wrap_module
 
 from .history import History, accum_in_tree, accum_histories_in_tree
 
 from . import mpi
 
-# error if old dependencies are detected
-from . import _dependencies_check
-
 _hide_submodules(
     __name__,
     remove_self=False,
     ignore=["numbers", "types", "float", "dispatch", "errors"],
 )
```

### Comparing `netket-3.7/netket/utils/_dependencies_check.py` & `netket-3.8/netket/utils/_dependencies_check.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/array.py` & `netket-3.8/netket/utils/array.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 
+from netket.utils import module_version
+
 from .types import Array, DType, Shape
 from .struct import dataclass
 
+# TODO keep only  jax>=0.4 is required
+if module_version("jax") >= (0, 4, 0):
+    import jax
+
+    JaxArray = jax.Array
+else:
+    # pre jax 0.4
+    import jaxlib
+
+    JaxArray = jaxlib.xla_extension.DeviceArray
+
 
 @dataclass(cache_hash=True)
 class HashableArray:
     """
     This class wraps a numpy or jax array in order to make it hashable and
     equality comparable (which is necessary since a well-defined hashable object
     needs to satisfy :code:`obj1 == obj2` whenever :code:`hash(obj1) == hash(obj2)`.
@@ -31,15 +44,19 @@
     wrapped: Array
     """The wrapped array. Note that this array is read-only."""
 
     def __pre_init__(self, wrapped):
         if isinstance(wrapped, HashableArray):
             wrapped = wrapped.wrapped
         else:
-            wrapped = wrapped.copy()
+            if isinstance(wrapped, JaxArray):
+                # __array__ only works if it's a numpy array.
+                wrapped = np.array(wrapped)
+            else:
+                wrapped = wrapped.copy()
             if isinstance(wrapped, np.ndarray):
                 wrapped.flags.writeable = False
 
         return (wrapped,), {}
 
     def __hash__(self):
         return hash(self.wrapped.tobytes())
```

### Comparing `netket-3.7/netket/utils/config_flags.py` & `netket-3.8/netket/utils/config_flags.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/deprecation.py` & `netket-3.8/netket/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/dispatch.py` & `netket-3.8/netket/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/errors.py` & `netket-3.8/netket/utils/errors.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/float.py` & `netket-3.8/netket/utils/float.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/history.py` & `netket-3.8/netket/utils/history.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/jax.py` & `netket-3.8/netket/utils/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/moduletools.py` & `netket-3.8/netket/utils/moduletools.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/numbers.py` & `netket-3.8/netket/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/optional_deps.py` & `netket-3.8/netket/utils/optional_deps.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/partial.py` & `netket-3.8/netket/utils/partial.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/seed.py` & `netket-3.8/netket/utils/seed.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/summation.py` & `netket-3.8/netket/utils/summation.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/types.py` & `netket-3.8/netket/utils/types.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/version_check.py` & `netket-3.8/netket/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/__init__.py` & `netket-3.8/netket/utils/group/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/_group.py` & `netket-3.8/netket/utils/group/_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/_permutation_group.py` & `netket-3.8/netket/utils/group/_permutation_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/_point_group.py` & `netket-3.8/netket/utils/group/_point_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/_semigroup.py` & `netket-3.8/netket/utils/group/_semigroup.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/axial.py` & `netket-3.8/netket/utils/group/axial.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/cubic.py` & `netket-3.8/netket/utils/group/cubic.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/icosa.py` & `netket-3.8/netket/utils/group/icosa.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/group/planar.py` & `netket-3.8/netket/utils/group/planar.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/model_frameworks/__init__.py` & `netket-3.8/netket/utils/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/model_frameworks/base.py` & `netket-3.8/netket/utils/model_frameworks/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/model_frameworks/flax.py` & `netket-3.8/netket/utils/model_frameworks/flax.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/model_frameworks/haiku.py` & `netket-3.8/netket/utils/model_frameworks/haiku.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/model_frameworks/jax.py` & `netket-3.8/netket/utils/model_frameworks/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/mpi/__init__.py` & `netket-3.8/netket/utils/mpi/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/mpi/mpi.py` & `netket-3.8/netket/utils/mpi/mpi.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/mpi/primitives.py` & `netket-3.8/netket/utils/mpi/primitives.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/struct/__init__.py` & `netket-3.8/netket/utils/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/struct/dataclass.py` & `netket-3.8/netket/utils/struct/dataclass.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/utils/struct/utils.py` & `netket-3.8/netket/utils/struct/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/__init__.py` & `netket-3.8/netket/vqs/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/base.py` & `netket-3.8/netket/vqs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import jax
 import jax.numpy as jnp
 from jax.nn.initializers import normal
 
 import flax
 from flax.core.frozen_dict import FrozenDict
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 import netket.jax as nkjax
 from netket.operator import AbstractOperator, Squared
 from netket.hilbert import AbstractHilbert
 from netket.utils.types import PyTree, PRNGKeyT, NNInitFunc
 from netket.utils.dispatch import dispatch, TrueT, FalseT
 from netket.stats import Stats
```

### Comparing `netket-3.7/netket/vqs/experimental.py` & `netket-3.8/netket/vqs/experimental.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/exact/__init__.py` & `netket-3.8/netket/vqs/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/exact/expect.py` & `netket-3.8/netket/vqs/exact/expect.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from functools import partial, lru_cache
 from typing import Callable, Tuple
 
 import jax
 from jax import numpy as jnp
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket import jax as nkjax
 from netket.operator import Squared
 from netket.stats import Stats
 from netket.utils.types import PyTree
 from netket.utils.dispatch import dispatch, TrueT
```

### Comparing `netket-3.7/netket/vqs/exact/state.py` & `netket-3.8/netket/vqs/exact/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Any, Callable, Dict, Optional
 
 import jax
 from jax import numpy as jnp
 
 import flax
 from flax import serialization
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket import jax as nkjax
 from netket import nn
 from netket.hilbert import AbstractHilbert
 from netket.utils import maybe_wrap_module, wrap_afun, wrap_to_support_scalar
 from netket.utils.types import PyTree, SeedT, NNInitFunc
 from netket.optimizer import LinearOperator
@@ -279,25 +279,27 @@
         if self._array is None and normalize:
             self._array = nn.to_array(
                 self.hilbert,
                 self._apply_fun,
                 self.variables,
                 normalize=normalize,
                 allgather=allgather,
+                chunk_size=self.chunk_size,
             )
 
         if normalize:
             arr = self._array
         else:
             arr = nn.to_array(
                 self.hilbert,
                 self._apply_fun,
                 self.variables,
                 normalize=normalize,
                 allgather=allgather,
+                chunk_size=self.chunk_size,
             )
 
         return arr
 
     def probability_distribution(self):
         if self._pdf is None:
             self._pdf = jnp.abs(self.to_array()) ** 2
```

### Comparing `netket-3.7/netket/vqs/mc/__init__.py` & `netket-3.8/netket/vqs/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/common.py` & `netket-3.8/netket/vqs/mc/common.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/kernels.py` & `netket-3.8/netket/vqs/mc/kernels.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_mixed_state/__init__.py` & `netket-3.8/netket/vqs/mc/mc_mixed_state/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_mixed_state/expect.py` & `netket-3.8/netket/vqs/mc/mc_mixed_state/expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_mixed_state/expect_chunked.py` & `netket-3.8/netket/vqs/mc/mc_mixed_state/expect_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py` & `netket-3.8/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_mixed_state/state.py` & `netket-3.8/netket/vqs/mc/mc_mixed_state/state.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_state/__init__.py` & `netket-3.8/netket/vqs/mc/mc_state/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_state/expect.py` & `netket-3.8/netket/vqs/mc/mc_state/expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_state/expect_chunked.py` & `netket-3.8/netket/vqs/mc/mc_state/expect_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.7/netket/vqs/mc/mc_state/expect_forces.py` & `netket-3.8/netket/vqs/mc/mc_state/expect_forces.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from functools import partial
 from typing import Callable, Tuple
 
 import jax
 from jax import numpy as jnp
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket import jax as nkjax
 from netket.stats import Stats, statistics
 from netket.utils import mpi
 from netket.utils.types import PyTree
 from netket.utils.dispatch import dispatch
```

### Comparing `netket-3.7/netket/vqs/mc/mc_state/expect_forces_chunked.py` & `netket-3.8/netket/vqs/mc/mc_state/expect_forces_chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from functools import partial
 from typing import Any, Callable, Tuple
 import warnings
 
 import jax
 from jax import numpy as jnp
 from jax import tree_map
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket import jax as nkjax
 from netket.operator import AbstractOperator
 from netket.stats import Stats, statistics
 from netket.utils import mpi
 from netket.utils.types import PyTree
```

### Comparing `netket-3.7/netket/vqs/mc/mc_state/expect_grad.py` & `netket-3.8/netket/vqs/mc/mc_state/expect_grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from functools import partial
 from typing import Callable, Tuple
 
 import jax
 from jax import numpy as jnp
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket import jax as nkjax
 from netket import config
 from netket.stats import Stats
 from netket.utils import mpi
 from netket.utils.types import PyTree
 from netket.utils.dispatch import TrueT, FalseT
```

### Comparing `netket-3.7/netket/vqs/mc/mc_state/expect_grad_chunked.py` & `netket-3.8/netket/vqs/mc/mc_state/expect_grad_chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from typing import Any, Tuple
 import warnings
 
 import jax
 from jax import numpy as jnp
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket.operator import AbstractOperator
 from netket.stats import Stats
 from netket.utils.types import PyTree
 from netket.utils.dispatch import TrueT, Bool
 
 from netket.vqs import expect_and_grad, expect_and_forces
```

### Comparing `netket-3.7/netket/vqs/mc/mc_state/state.py` & `netket-3.8/netket/vqs/mc/mc_state/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import numpy as np
 
 import jax
 from jax import numpy as jnp
 
 import flax
 from flax import serialization
-from flax.core.scope import CollectionFilter
+from flax.core.scope import CollectionFilter, DenyList  # noqa: F401
 
 from netket import jax as nkjax
 from netket import nn
 from netket.stats import Stats
 from netket.operator import AbstractOperator, Squared
 from netket.sampler import Sampler, SamplerState
 from netket.utils import (
@@ -647,16 +647,21 @@
 
         Returns:
             nk.optimizer.LinearOperator: A linear operator representing the quantum geometric tensor.
         """
         return qgt_T(self)
 
     def to_array(self, normalize: bool = True) -> jnp.ndarray:
+
         return nn.to_array(
-            self.hilbert, self._apply_fun, self.variables, normalize=normalize
+            self.hilbert,
+            self._apply_fun,
+            self.variables,
+            normalize=normalize,
+            chunk_size=self.chunk_size,
         )
 
     def __repr__(self):
         return (
             "MCState("
             + "\n  hilbert = {},".format(self.hilbert)
             + "\n  sampler = {},".format(self.sampler)
```

### Comparing `netket-3.7/.gitignore` & `netket-3.8/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __pycache__/
 *.py[cod]
 netket.egg-info/
 pip-wheel-metadata
 .ipynb_checkpoints
 .pytest_cache
 .mypy_cache
+.virtual_documents
 oldest_requirements.txt
 
 # Packages #
 ############
 # it's better to unpack these files and commit the raw source
 # git has its own built in compression methods
 *.7z
```

### Comparing `netket-3.7/LICENSE` & `netket-3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netket-3.7/README.md` & `netket-3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # __NetKet__
 
 [![Release](https://img.shields.io/github/release/netket/netket.svg)](https://github.com/netket/netket/releases)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/netket/badges/version.svg)](https://anaconda.org/conda-forge/netket)
 [![Paper (v3)](https://img.shields.io/badge/paper%20%28v3%29-arXiv%3A2112.10526-B31B1B)](https://scipost.org/SciPostPhysCodeb.7/pdf)
 [![codecov](https://codecov.io/gh/netket/netket/branch/master/graph/badge.svg?token=gzcOlpO5lB)](https://codecov.io/gh/netket/netket)
-[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/mlquantum/shared_invite/zt-19wibmfdv-LLRI6i43wrLev6oQX0OfOw) 
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/mlquantum/shared_invite/zt-19wibmfdv-LLRI6i43wrLev6oQX0OfOw)
 
 NetKet is an open-source project delivering cutting-edge methods for the study
 of many-body quantum systems with artificial neural networks and machine learning techniques.
 It is a Python library built on [JAX](https://github.com/google/jax).
 
 - **Homepage:** <https://www.netket.org>
 - **Citing:** <https://www.netket.org/cite/>
@@ -74,20 +74,20 @@
 ```
 
 ### Installation on Windows
 **WARNING:** Windows support is **experimental**, and you should expect suboptimal performance.
 
 We suggest to use Windows Subsystem for Linux (WSL), on which you can install NetKet following the same instructions as above, and CUDA and MPI work as intended.
 
-However, if you just want to quickly get started with NetKet, it is also possible to install it natively on Windows. First, download an unofficial `jaxlib` wheel from [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder):
+However, if you just want to quickly get started with NetKet, it is also possible to install it natively on Windows. First, download an unofficial build of `jax` from [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder):
 ```sh
 pip install --upgrade pip
-pip install jaxlib -f https://whls.blob.core.windows.net/unstable/index.html
+pip install "jax[cpu]===0.3.25" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 ```
-Alternatively, you may specify a wheel version with CUDA support.
+Alternatively, you may specify a version with CUDA support.
 
 Then install NetKet as usual:
 ```sh
 pip install --upgrade netket
 ```
 
 If you want MPI support, please follow the discussion in [mpi4jax](https://github.com/mpi4jax/mpi4jax/issues/24).
```

### Comparing `netket-3.7/pyproject.toml` & `netket-3.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 dynamic = ["version"]
 
 requires-python = ">=3.7"
 dependencies = [
     "numpy~=1.20",
     "scipy>=1.5.3, <2",
     "tqdm>=4.60, <5",
-    "plum-dispatch>=1.5.1, <2",
-    "numba>=0.52, <0.57",
+    "plum-dispatch>=1.5.1, <3",
+    "numba>=0.52, <0.58",
     "igraph>=0.9.8, <0.11.0",
     "jax>=0.3.16, <0.5",
     "jaxlib>=0.3.15, <0.5",
     "flax>=0.6, <0.7",
     "orjson>=3.4, <4",
     "optax>=0.1.3, <0.2",
     "numba4jax>=0.0.10, <0.1",
@@ -52,27 +52,39 @@
     ]
 extra = [
     "tensorboardx>=2.0.0",
     "openfermion>=1.0.0",
     "h5py>=3.7.0",
     ]
 dev = [
+    "networkx>=2.4, <4",
+    "matplotlib>=3",
     "pytest>=6",
     "pytest-xdist[psutil]>=2",
     "pytest-cov>=2.10.1",
     "pytest-json-report>=1.3",
     "coverage>=5",
-    "networkx>=2.4, <4",
     "pre-commit>=2.7",
     "black==22.10.0",
     "flake8==6.0.0; python_version >= '3.8'",
     "flake8==5.0.4; python_version < '3.8'",
     "wheel",
     "build",
 ]
+docs = [
+    "Sphinx>=5.3,<7.1",
+    "sphinx-autodoc-typehints~=1.22",
+    "sphinxcontrib-fulltoc~=1.2.0",
+    "sphinxcontrib-jsmath~=1.0.1",
+    "sphinxcontrib-napoleon==0.7",
+    "myst-parser~=0.18.1",
+    "nbsphinx~=0.9.1",
+    "myst-nb~=0.17.1",
+    "sphinx-book-theme~=1.0.1",
+]
 
 [project.urls]
  homepage = "https://www.netket.org"
  documentation = "https://netket.readthedocs.io/en/latest/#"
  repository = "https://github.com/netket/netket"
  changelog = "https://netket.readthedocs.io/en/latest/docs/changelog.html"
```

### Comparing `netket-3.7/PKG-INFO` & `netket-3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetKet
-Version: 3.7
+Version: 3.8
 Summary: Netket : Machine Learning toolbox for many-body quantum systems.
 Project-URL: homepage, https://www.netket.org
 Project-URL: documentation, https://netket.readthedocs.io/en/latest/#
 Project-URL: repository, https://github.com/netket/netket
 Project-URL: changelog, https://netket.readthedocs.io/en/latest/docs/changelog.html
 Author: Giuseppe Carleo, Filippo Vicentini, The NetKet authors
 License: Apache 2.0
@@ -19,34 +19,45 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Requires-Dist: flax<0.7,>=0.6
 Requires-Dist: igraph<0.11.0,>=0.9.8
 Requires-Dist: jax<0.5,>=0.3.16
 Requires-Dist: jaxlib<0.5,>=0.3.15
 Requires-Dist: numba4jax<0.1,>=0.0.10
-Requires-Dist: numba<0.57,>=0.52
+Requires-Dist: numba<0.58,>=0.52
 Requires-Dist: numpy~=1.20
 Requires-Dist: optax<0.2,>=0.1.3
 Requires-Dist: orjson<4,>=3.4
-Requires-Dist: plum-dispatch<2,>=1.5.1
+Requires-Dist: plum-dispatch<3,>=1.5.1
 Requires-Dist: scipy<2,>=1.5.3
 Requires-Dist: tqdm<5,>=4.60
 Provides-Extra: dev
 Requires-Dist: black==22.10.0; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: coverage>=5; extra == 'dev'
 Requires-Dist: flake8==5.0.4; python_version < '3.8' and extra == 'dev'
 Requires-Dist: flake8==6.0.0; python_version >= '3.8' and extra == 'dev'
+Requires-Dist: matplotlib>=3; extra == 'dev'
 Requires-Dist: networkx<4,>=2.4; extra == 'dev'
 Requires-Dist: pre-commit>=2.7; extra == 'dev'
 Requires-Dist: pytest-cov>=2.10.1; extra == 'dev'
 Requires-Dist: pytest-json-report>=1.3; extra == 'dev'
 Requires-Dist: pytest-xdist[psutil]>=2; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: myst-nb~=0.17.1; extra == 'docs'
+Requires-Dist: myst-parser~=0.18.1; extra == 'docs'
+Requires-Dist: nbsphinx~=0.9.1; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints~=1.22; extra == 'docs'
+Requires-Dist: sphinx-book-theme~=1.0.1; extra == 'docs'
+Requires-Dist: sphinx<7.1,>=5.3; extra == 'docs'
+Requires-Dist: sphinxcontrib-fulltoc~=1.2.0; extra == 'docs'
+Requires-Dist: sphinxcontrib-jsmath~=1.0.1; extra == 'docs'
+Requires-Dist: sphinxcontrib-napoleon==0.7; extra == 'docs'
 Provides-Extra: extra
 Requires-Dist: h5py>=3.7.0; extra == 'extra'
 Requires-Dist: openfermion>=1.0.0; extra == 'extra'
 Requires-Dist: tensorboardx>=2.0.0; extra == 'extra'
 Provides-Extra: mpi
 Requires-Dist: mpi4jax<0.4,>=0.3.9; extra == 'mpi'
 Requires-Dist: mpi4py<4,>=3.0.1; extra == 'mpi'
@@ -58,15 +69,15 @@
 
 # __NetKet__
 
 [![Release](https://img.shields.io/github/release/netket/netket.svg)](https://github.com/netket/netket/releases)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/netket/badges/version.svg)](https://anaconda.org/conda-forge/netket)
 [![Paper (v3)](https://img.shields.io/badge/paper%20%28v3%29-arXiv%3A2112.10526-B31B1B)](https://scipost.org/SciPostPhysCodeb.7/pdf)
 [![codecov](https://codecov.io/gh/netket/netket/branch/master/graph/badge.svg?token=gzcOlpO5lB)](https://codecov.io/gh/netket/netket)
-[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/mlquantum/shared_invite/zt-19wibmfdv-LLRI6i43wrLev6oQX0OfOw) 
+[![Slack](https://img.shields.io/badge/slack-chat-green.svg)](https://join.slack.com/t/mlquantum/shared_invite/zt-19wibmfdv-LLRI6i43wrLev6oQX0OfOw)
 
 NetKet is an open-source project delivering cutting-edge methods for the study
 of many-body quantum systems with artificial neural networks and machine learning techniques.
 It is a Python library built on [JAX](https://github.com/google/jax).
 
 - **Homepage:** <https://www.netket.org>
 - **Citing:** <https://www.netket.org/cite/>
@@ -128,20 +139,20 @@
 ```
 
 ### Installation on Windows
 **WARNING:** Windows support is **experimental**, and you should expect suboptimal performance.
 
 We suggest to use Windows Subsystem for Linux (WSL), on which you can install NetKet following the same instructions as above, and CUDA and MPI work as intended.
 
-However, if you just want to quickly get started with NetKet, it is also possible to install it natively on Windows. First, download an unofficial `jaxlib` wheel from [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder):
+However, if you just want to quickly get started with NetKet, it is also possible to install it natively on Windows. First, download an unofficial build of `jax` from [cloudhan/jax-windows-builder](https://github.com/cloudhan/jax-windows-builder):
 ```sh
 pip install --upgrade pip
-pip install jaxlib -f https://whls.blob.core.windows.net/unstable/index.html
+pip install "jax[cpu]===0.3.25" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 ```
-Alternatively, you may specify a wheel version with CUDA support.
+Alternatively, you may specify a version with CUDA support.
 
 Then install NetKet as usual:
 ```sh
 pip install --upgrade netket
 ```
 
 If you want MPI support, please follow the discussion in [mpi4jax](https://github.com/mpi4jax/mpi4jax/issues/24).
```


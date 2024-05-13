# Comparing `tmp/lakers_python-0.2.1.tar.gz` & `tmp/lakers_python-0.3.0.tar.gz`

## Comparing `lakers_python-0.2.1.tar` & `lakers_python-0.3.0.tar`

### file list

```diff
@@ -1,151 +1,149 @@
--rw-r--r--   0     1001      127      384 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/Cargo.toml
--rw-r--r--   0     1001      127     1580 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/build.rs
--rw-r--r--   0     1001      127     2050 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h
--rw-r--r--   0     1001      127    10187 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs
--rw-r--r--   0     1001      127      771 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile
--rw-r--r--   0     1001      127     1217 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal
--rw-r--r--   0     1001      127     4213 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h
--rw-r--r--   0     1001      127     4680 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c
--rw-r--r--   0     1001      127    13789 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h
--rw-r--r--   0     1001      127     3989 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h
--rw-r--r--   0     1001      127     6951 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h
--rw-r--r--   0     1001      127    18924 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h
--rw-r--r--   0     1001      127     7180 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h
--rw-r--r--   0     1001      127    12210 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h
--rw-r--r--   0     1001      127     5299 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h
--rw-r--r--   0     1001      127     5336 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h
--rw-r--r--   0     1001      127     4848 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h
--rw-r--r--   0     1001      127    17291 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h
--rw-r--r--   0     1001      127     5103 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h
--rw-r--r--   0     1001      127    28262 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h
--rw-r--r--   0     1001      127     8030 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h
--rw-r--r--   0     1001      127    12591 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h
--rw-r--r--   0     1001      127    11841 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h
--rw-r--r--   0     1001      127    13273 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h
--rw-r--r--   0     1001      127     6273 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h
--rw-r--r--   0     1001      127    13454 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h
--rw-r--r--   0     1001      127     5126 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h
--rw-r--r--   0     1001      127     3832 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h
--rw-r--r--   0     1001      127     8772 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h
--rw-r--r--   0     1001      127    19639 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h
--rw-r--r--   0     1001      127     4757 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h
--rw-r--r--   0     1001      127    19193 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h
--rw-r--r--   0     1001      127    12890 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h
--rw-r--r--   0     1001      127    13780 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h
--rw-r--r--   0     1001      127     3376 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h
--rw-r--r--   0     1001      127     5101 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h
--rw-r--r--   0     1001      127     6138 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h
--rw-r--r--   0     1001      127     4247 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h
--rw-r--r--   0     1001      127    11821 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h
--rw-r--r--   0     1001      127     3374 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h
--rw-r--r--   0     1001      127     5259 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h
--rw-r--r--   0     1001      127    10891 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h
--rw-r--r--   0     1001      127     5154 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h
--rw-r--r--   0     1001      127     7450 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h
--rw-r--r--   0     1001      127     4998 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h
--rw-r--r--   0     1001      127     4170 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h
--rw-r--r--   0     1001      127    19714 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h
--rw-r--r--   0     1001      127     8213 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h
--rw-r--r--   0     1001      127     9721 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h
--rw-r--r--   0     1001      127    16219 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h
--rw-r--r--   0     1001      127     7582 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h
--rw-r--r--   0     1001      127     7921 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h
--rw-r--r--   0     1001      127    34649 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h
--rw-r--r--   0     1001      127    23132 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h
--rw-r--r--   0     1001      127    17872 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h
--rw-r--r--   0     1001      127     4401 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h
--rw-r--r--   0     1001      127     3641 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h
--rw-r--r--   0     1001      127     4914 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h
--rw-r--r--   0     1001      127    17381 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h
--rw-r--r--   0     1001      127     4168 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h
--rw-r--r--   0     1001      127     7180 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h
--rw-r--r--   0     1001      127     4233 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h
--rw-r--r--   0     1001      127     3536 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h
--rw-r--r--   0     1001      127     3700 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h
--rw-r--r--   0     1001      127     8494 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h
--rw-r--r--   0     1001      127     9900 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h
--rw-r--r--   0     1001      127     4089 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h
--rw-r--r--   0     1001      127     3582 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h
--rw-r--r--   0     1001      127     4187 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h
--rw-r--r--   0     1001      127     9241 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h
--rw-r--r--   0     1001      127     5012 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h
--rw-r--r--   0     1001      127     4816 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h
--rw-r--r--   0     1001      127     4021 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h
--rw-r--r--   0     1001      127     4605 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h
--rw-r--r--   0     1001      127     9188 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h
--rw-r--r--   0     1001      127     7156 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h
--rw-r--r--   0     1001      127     4487 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h
--rw-r--r--   0     1001      127     5729 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h
--rw-r--r--   0     1001      127     3606 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h
--rw-r--r--   0     1001      127     5696 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h
--rw-r--r--   0     1001      127     3287 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h
--rw-r--r--   0     1001      127     5074 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h
--rw-r--r--   0     1001      127     5028 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h
--rw-r--r--   0     1001      127     3426 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h
--rw-r--r--   0     1001      127     5532 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h
--rw-r--r--   0     1001      127     3458 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h
--rw-r--r--   0     1001      127     3885 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h
--rw-r--r--   0     1001      127     8745 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h
--rw-r--r--   0     1001      127     3742 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h
--rw-r--r--   0     1001      127     4544 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h
--rw-r--r--   0     1001      127     5141 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h
--rw-r--r--   0     1001      127     5670 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h
--rw-r--r--   0     1001      127     4277 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h
--rw-r--r--   0     1001      127   297096 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   296510 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   297096 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   296510 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   296510 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
--rw-r--r--   0     1001      127   297096 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib
--rw-r--r--   0     1001      127   295748 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   295162 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   295748 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   295162 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0     1001      127   295162 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
--rw-r--r--   0     1001      127   295748 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib
--rw-r--r--   0     1001      127     1501 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt
--rw-r--r--   0     1001      127     1501 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt
--rw-r--r--   0     1001      127      136 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/README.md
--rw-r--r--   0     1001      127      753 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-rustcrypto/Cargo.toml
--rw-r--r--   0     1001      127     5225 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-rustcrypto/src/lib.rs
--rw-r--r--   0     1001      127      644 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lib/Cargo.toml
--rw-r--r--   0     1001      127    57886 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lib/src/edhoc.rs
--rw-r--r--   0     1001      127    25413 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lib/src/lib.rs
--rw-r--r--   0     1001      127     4656 2024-03-05 16:50:42.000000 lakers_python-0.2.1/README.md
--rw-r--r--   0     1001      127     1464 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/Cargo.toml
--rw-r--r--   0     1001      127      290 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/.cargo/config.toml
--rw-r--r--   0     1001      127     1794 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/src/lib.rs
--rw-r--r--   0     1001      127      387 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/Cargo.toml
--rw-r--r--   0     1001      127      611 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/cbindgen.toml
--rw-r--r--   0     1001      127     7125 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/src/authenticator.rs
--rw-r--r--   0     1001      127     7448 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/src/device.rs
--rw-r--r--   0     1001      127     3245 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/src/lib.rs
--rw-r--r--   0     1001      127    13060 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/src/server.rs
--rw-r--r--   0     1001      127     7454 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/src/shared.rs
--rw-r--r--   0     1001      127     3766 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/lakers-ead-authz/src/test_vectors.rs
--rw-r--r--   0     1001      127      446 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/Cargo.toml
--rw-r--r--   0     1001      127       71 2024-03-05 16:50:42.000000 lakers_python-0.2.1/ead/src/lib.rs
--rw-r--r--   0     1001      127      520 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/Cargo.toml
--rw-r--r--   0     1001      127      832 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/cbindgen.toml
--rw-r--r--   0     1001      127     3085 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/src/cred.rs
--rw-r--r--   0     1001      127     2110 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/src/crypto.rs
--rw-r--r--   0     1001      127    27058 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/src/lib.rs
--rw-r--r--   0     1001      127     1511 2024-03-05 16:50:42.000000 lakers_python-0.2.1/shared/src/python_bindings.rs
--rw-r--r--   0     1001      127      391 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-psa/Cargo.toml
--rw-r--r--   0     1001      127    10616 2024-03-05 16:50:42.000000 lakers_python-0.2.1/crypto/lakers-crypto-psa/src/lib.rs
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 lakers_python-0.2.1/lakers-python/Cargo.toml
--rw-r--r--   0     1001      127      764 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/README.md
--rw-r--r--   0     1001      127     1392 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/ead_authz/authenticator.rs
--rw-r--r--   0     1001      127     2133 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/ead_authz/device.rs
--rw-r--r--   0     1001      127      107 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/ead_authz/mod.rs
--rw-r--r--   0     1001      127     2413 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/ead_authz/server.rs
--rw-r--r--   0     1001      127     5738 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/initiator.rs
--rw-r--r--   0     1001      127     2843 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/lib.rs
--rw-r--r--   0     1001      127     4482 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/src/responder.rs
--rw-r--r--   0     1001      127     4476 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/test/test_ead_authz.py
--rw-r--r--   0     1001      127     3176 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/test/test_lakers.py
--rw-r--r--   0     1001      127        6 2024-03-05 16:50:42.000000 lakers_python-0.2.1/lakers-python/test_requirements.txt
--rw-r--r--   0     1001      127    63093 2024-03-05 16:51:22.000000 lakers_python-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     2274 1970-01-01 00:00:00.000000 lakers_python-0.2.1/Cargo.toml
--rw-r--r--   0        0        0      141 1970-01-01 00:00:00.000000 lakers_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 lakers_python-0.2.1/PKG-INFO
+-rw-r--r--   0   671610   202045      384 2024-01-16 08:08:59.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/Cargo.toml
+-rw-r--r--   0   671610   202045     1580 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/build.rs
+-rw-r--r--   0   671610   202045     2050 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h
+-rw-r--r--   0   671610   202045    10187 2024-04-05 13:22:30.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs
+-rw-r--r--   0   671610   202045      771 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile
+-rw-r--r--   0   671610   202045     1217 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal
+-rw-r--r--   0   671610   202045     4213 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h
+-rw-r--r--   0   671610   202045     4680 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c
+-rw-r--r--   0   671610   202045    13789 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h
+-rw-r--r--   0   671610   202045     3989 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h
+-rw-r--r--   0   671610   202045     6951 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h
+-rw-r--r--   0   671610   202045    18924 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h
+-rw-r--r--   0   671610   202045     7180 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h
+-rw-r--r--   0   671610   202045    12210 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h
+-rw-r--r--   0   671610   202045     5299 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h
+-rw-r--r--   0   671610   202045     5336 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h
+-rw-r--r--   0   671610   202045     4848 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h
+-rw-r--r--   0   671610   202045    17291 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h
+-rw-r--r--   0   671610   202045     5103 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h
+-rw-r--r--   0   671610   202045    28262 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h
+-rw-r--r--   0   671610   202045     8030 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h
+-rw-r--r--   0   671610   202045    12591 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h
+-rw-r--r--   0   671610   202045    11841 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h
+-rw-r--r--   0   671610   202045    13273 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h
+-rw-r--r--   0   671610   202045     6273 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h
+-rw-r--r--   0   671610   202045    13454 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h
+-rw-r--r--   0   671610   202045     5126 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h
+-rw-r--r--   0   671610   202045     3832 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h
+-rw-r--r--   0   671610   202045     8772 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h
+-rw-r--r--   0   671610   202045    19639 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h
+-rw-r--r--   0   671610   202045     4757 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h
+-rw-r--r--   0   671610   202045    19193 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h
+-rw-r--r--   0   671610   202045    12890 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h
+-rw-r--r--   0   671610   202045    13780 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h
+-rw-r--r--   0   671610   202045     3376 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h
+-rw-r--r--   0   671610   202045     5101 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h
+-rw-r--r--   0   671610   202045     6138 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h
+-rw-r--r--   0   671610   202045     4247 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h
+-rw-r--r--   0   671610   202045    11821 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h
+-rw-r--r--   0   671610   202045     3374 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h
+-rw-r--r--   0   671610   202045     5259 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h
+-rw-r--r--   0   671610   202045    10891 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h
+-rw-r--r--   0   671610   202045     5154 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h
+-rw-r--r--   0   671610   202045     7450 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h
+-rw-r--r--   0   671610   202045     4998 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h
+-rw-r--r--   0   671610   202045     4170 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h
+-rw-r--r--   0   671610   202045    19714 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h
+-rw-r--r--   0   671610   202045     8213 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h
+-rw-r--r--   0   671610   202045     9721 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h
+-rw-r--r--   0   671610   202045    16219 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h
+-rw-r--r--   0   671610   202045     7582 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h
+-rw-r--r--   0   671610   202045     7921 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h
+-rw-r--r--   0   671610   202045    34649 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h
+-rw-r--r--   0   671610   202045    23132 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h
+-rw-r--r--   0   671610   202045    17872 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h
+-rw-r--r--   0   671610   202045     4401 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h
+-rw-r--r--   0   671610   202045     3641 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h
+-rw-r--r--   0   671610   202045     4914 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h
+-rw-r--r--   0   671610   202045    17381 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h
+-rw-r--r--   0   671610   202045     4168 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h
+-rw-r--r--   0   671610   202045     7180 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h
+-rw-r--r--   0   671610   202045     4233 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h
+-rw-r--r--   0   671610   202045     3536 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h
+-rw-r--r--   0   671610   202045     3700 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h
+-rw-r--r--   0   671610   202045     8494 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h
+-rw-r--r--   0   671610   202045     9900 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h
+-rw-r--r--   0   671610   202045     4089 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h
+-rw-r--r--   0   671610   202045     3582 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h
+-rw-r--r--   0   671610   202045     4187 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h
+-rw-r--r--   0   671610   202045     9241 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h
+-rw-r--r--   0   671610   202045     5012 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h
+-rw-r--r--   0   671610   202045     4816 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h
+-rw-r--r--   0   671610   202045     4021 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h
+-rw-r--r--   0   671610   202045     4605 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h
+-rw-r--r--   0   671610   202045     9188 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h
+-rw-r--r--   0   671610   202045     7156 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h
+-rw-r--r--   0   671610   202045     4487 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h
+-rw-r--r--   0   671610   202045     5729 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h
+-rw-r--r--   0   671610   202045     3606 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h
+-rw-r--r--   0   671610   202045     5696 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h
+-rw-r--r--   0   671610   202045     3287 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h
+-rw-r--r--   0   671610   202045     5074 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h
+-rw-r--r--   0   671610   202045     5028 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h
+-rw-r--r--   0   671610   202045     3426 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h
+-rw-r--r--   0   671610   202045     5532 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h
+-rw-r--r--   0   671610   202045     3458 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h
+-rw-r--r--   0   671610   202045     3885 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h
+-rw-r--r--   0   671610   202045     8745 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h
+-rw-r--r--   0   671610   202045     3742 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h
+-rw-r--r--   0   671610   202045     4544 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h
+-rw-r--r--   0   671610   202045     5141 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h
+-rw-r--r--   0   671610   202045     5670 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h
+-rw-r--r--   0   671610   202045     4277 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h
+-rw-r--r--   0   671610   202045   297096 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   296510 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   297096 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   296510 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   296510 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
+-rw-r--r--   0   671610   202045   297096 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib
+-rw-r--r--   0   671610   202045   295748 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   295162 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   295748 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   295162 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0   671610   202045   295162 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
+-rw-r--r--   0   671610   202045   295748 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib
+-rw-r--r--   0   671610   202045     1501 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt
+-rw-r--r--   0   671610   202045     1501 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt
+-rw-r--r--   0   671610   202045      136 2024-01-16 08:08:59.000000 lakers_python-0.3.0/shared/README.md
+-rw-r--r--   0   671610   202045      753 2024-01-16 08:08:59.000000 lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/Cargo.toml
+-rw-r--r--   0   671610   202045     5225 2024-02-02 13:05:06.000000 lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/src/lib.rs
+-rw-r--r--   0   671610   202045      387 2024-02-16 09:54:33.000000 lakers_python-0.3.0/ead/lakers-ead-authz/Cargo.toml
+-rw-r--r--   0   671610   202045      633 2024-03-07 10:47:35.000000 lakers_python-0.3.0/ead/lakers-ead-authz/cbindgen.toml
+-rw-r--r--   0   671610   202045     7151 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/authenticator.rs
+-rw-r--r--   0   671610   202045     7458 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/device.rs
+-rw-r--r--   0   671610   202045     3522 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/lib.rs
+-rw-r--r--   0   671610   202045    13076 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/server.rs
+-rw-r--r--   0   671610   202045     7453 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/shared.rs
+-rw-r--r--   0   671610   202045     3766 2024-01-16 14:15:54.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/test_vectors.rs
+-rw-r--r--   0   671610   202045      618 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lib/Cargo.toml
+-rw-r--r--   0   671610   202045     6054 2024-04-05 13:20:00.000000 lakers_python-0.3.0/lib/README.md
+-rw-r--r--   0   671610   202045    58361 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lib/src/edhoc.rs
+-rw-r--r--   0   671610   202045    25819 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lib/src/lib.rs
+-rw-r--r--   0   671610   202045     1276 2024-04-05 13:20:00.000000 lakers_python-0.3.0/crypto/Cargo.toml
+-rw-r--r--   0   671610   202045      290 2023-05-09 08:42:52.000000 lakers_python-0.3.0/crypto/.cargo/config.toml
+-rw-r--r--   0   671610   202045     3039 2024-04-05 13:20:00.000000 lakers_python-0.3.0/crypto/src/lib.rs
+-rw-r--r--   0   671610   202045      574 2024-04-05 13:20:00.000000 lakers_python-0.3.0/shared/Cargo.toml
+-rw-r--r--   0   671610   202045      832 2024-03-07 15:22:47.000000 lakers_python-0.3.0/shared/cbindgen.toml
+-rw-r--r--   0   671610   202045     3081 2024-04-05 13:20:00.000000 lakers_python-0.3.0/shared/src/cred.rs
+-rw-r--r--   0   671610   202045     2110 2024-02-02 13:05:06.000000 lakers_python-0.3.0/shared/src/crypto.rs
+-rw-r--r--   0   671610   202045    32584 2024-05-13 12:19:21.000000 lakers_python-0.3.0/shared/src/lib.rs
+-rw-r--r--   0   671610   202045     1511 2024-02-29 11:00:51.000000 lakers_python-0.3.0/shared/src/python_bindings.rs
+-rw-r--r--   0   671610   202045      391 2024-01-16 08:08:59.000000 lakers_python-0.3.0/crypto/lakers-crypto-psa/Cargo.toml
+-rw-r--r--   0   671610   202045    10617 2024-03-13 14:06:27.000000 lakers_python-0.3.0/crypto/lakers-crypto-psa/src/lib.rs
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 lakers_python-0.3.0/lakers-python/Cargo.toml
+-rw-r--r--   0   671610   202045      764 2024-02-08 15:19:49.000000 lakers_python-0.3.0/lakers-python/README.md
+-rw-r--r--   0   671610   202045     1398 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/authenticator.rs
+-rw-r--r--   0   671610   202045     2139 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/device.rs
+-rw-r--r--   0   671610   202045      107 2024-02-29 11:00:51.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/mod.rs
+-rw-r--r--   0   671610   202045     2419 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/server.rs
+-rw-r--r--   0   671610   202045     6083 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/initiator.rs
+-rw-r--r--   0   671610   202045     3046 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/lib.rs
+-rw-r--r--   0   671610   202045     4915 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/responder.rs
+-rw-r--r--   0   671610   202045     4496 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/test/test_ead_authz.py
+-rw-r--r--   0   671610   202045     3152 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/test/test_lakers.py
+-rw-r--r--   0   671610   202045        6 2024-02-08 15:19:49.000000 lakers_python-0.3.0/lakers-python/test_requirements.txt
+-rw-r--r--   0   671610   202045    57821 2024-05-13 12:28:36.000000 lakers_python-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 lakers_python-0.3.0/Cargo.toml
+-rw-r--r--   0        0        0      141 1970-01-01 00:00:00.000000 lakers_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 lakers_python-0.3.0/PKG-INFO
```

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/build.rs` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/build.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt` & `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-rustcrypto/Cargo.toml` & `lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-rustcrypto/src/lib.rs` & `lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/lib/Cargo.toml` & `lakers_python-0.3.0/lib/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [package]
 name = "lakers"
 version.workspace = true
 edition = "2021"
 authors = ["Mališa Vučinić <malisa.vucinic@inria.fr>"]
 license.workspace = true
-description = "EDHOC implementation in Rust"
+description = "An implementation of EDHOC (RFC 9528)"
 repository.workspace = true
-readme = "../README.md"
+keywords.workspace = true
+categories.workspace = true
 
 [dependencies]
 lakers-shared.workspace = true
 
 [dev-dependencies]
-lakers-ead = { workspace = true, default-features = false }
+lakers-ead-authz = { workspace = true }
 lakers-crypto.workspace = true
 hexlit = "0.5.3"
 
 [features]
 # NOTE: the ead features are just needed for multiplexing tests
 default = [ "test-ead-none" ]
-test-ead-none = [ "lakers-ead/ead-none" ]
-test-ead-authz = [ "lakers-ead/ead-authz" ]
+test-ead-none = [ ]
+test-ead-authz = [ ]
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `lakers_python-0.2.1/lib/src/edhoc.rs` & `lakers_python-0.3.0/lib/src/edhoc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     state.prk_out
 }
 
 pub fn r_process_message_1(
     state: &ResponderStart,
     crypto: &mut impl CryptoTrait,
     message_1: &BufferMessage1,
-) -> Result<(ProcessingM1, Option<EADItem>), EDHOCError> {
+) -> Result<(ProcessingM1, ConnId, Option<EADItem>), EDHOCError> {
     // Step 1: decode message_1
     // g_x will be saved to the state
     if let Ok((method, suites_i, suites_i_len, g_x, c_i, ead_1)) = parse_message_1(message_1) {
         // verify that the method is supported
         if method == EDHOC_METHOD {
             // Step 2: verify that the selected cipher suite is supported
             if suites_i[suites_i_len - 1] == EDHOC_SUPPORTED_SUITES[0] {
@@ -74,14 +74,15 @@
                     ProcessingM1 {
                         y: state.y,
                         g_y: state.g_y,
                         c_i,
                         g_x,
                         h_message_1,
                     },
+                    c_i,
                     ead_1,
                 ))
             } else {
                 Err(EDHOCError::UnsupportedCipherSuite)
             }
         } else {
             Err(EDHOCError::UnsupportedMethod)
@@ -92,15 +93,15 @@
 }
 
 pub fn r_prepare_message_2(
     state: &ProcessingM1,
     crypto: &mut impl CryptoTrait,
     cred_r: CredentialRPK,
     r: &BytesP256ElemLen, // R's static private DH key
-    c_r: u8,
+    c_r: ConnId,
     cred_transfer: CredentialTransfer,
     ead_2: &Option<EADItem>,
 ) -> Result<(WaitM3, BufferMessage2), EDHOCError> {
     // compute TH_2
     let th_2 = compute_th_2(crypto, &state.g_y, &state.h_message_1);
 
     // compute prk_3e2m
@@ -130,15 +131,15 @@
     // step is actually from processing of message_3
     // but we do it here to avoid storing plaintext_2 in State
     let th_3 = compute_th_3(crypto, &th_2, &plaintext_2, cred_r.value.as_slice());
 
     let mut ct: BufferCiphertext2 = BufferCiphertext2::new();
     ct.fill_with_slice(plaintext_2.as_slice()).unwrap(); // TODO(hax): can we prove with hax that this won't panic since they use the same underlying buffer length?
 
-    let ciphertext_2 = encrypt_decrypt_ciphertext_2(crypto, &prk_2e, &th_2, ct);
+    let ciphertext_2 = encrypt_decrypt_ciphertext_2(crypto, &prk_2e, &th_2, &ct);
 
     ct.fill_with_slice(ciphertext_2.as_slice()).unwrap(); // TODO(hax): same as just above.
 
     let message_2 = encode_message_2(&state.g_y, &ct);
 
     Ok((
         WaitM3 {
@@ -265,15 +266,15 @@
         Err(EDHOCError::MacVerificationFailed)
     }
 }
 
 pub fn i_prepare_message_1(
     state: &InitiatorStart,
     crypto: &mut impl CryptoTrait,
-    c_i: u8,
+    c_i: ConnId,
     ead_1: &Option<EADItem>, // FIXME: make it a list of EADItem
 ) -> Result<(WaitM2, BufferMessage1), EDHOCError> {
     // Encode message_1 as a sequence of CBOR encoded data items as specified in Section 5.2.1
     let message_1 = encode_message_1(
         EDHOC_METHOD,
         &state.suites_i,
         state.suites_i_len,
@@ -298,23 +299,23 @@
 }
 
 // returns c_r
 pub fn i_parse_message_2<'a>(
     state: &WaitM2,
     crypto: &mut impl CryptoTrait,
     message_2: &BufferMessage2,
-) -> Result<(ProcessingM2, u8, CredentialRPK, Option<EADItem>), EDHOCError> {
+) -> Result<(ProcessingM2, ConnId, CredentialRPK, Option<EADItem>), EDHOCError> {
     let res = parse_message_2(message_2);
     if let Ok((g_y, ciphertext_2)) = res {
         let th_2 = compute_th_2(crypto, &g_y, &state.h_message_1);
 
         // compute prk_2e
         let prk_2e = compute_prk_2e(crypto, &state.x, &g_y, &th_2);
 
-        let plaintext_2 = encrypt_decrypt_ciphertext_2(crypto, &prk_2e, &th_2, ciphertext_2);
+        let plaintext_2 = encrypt_decrypt_ciphertext_2(crypto, &prk_2e, &th_2, &ciphertext_2);
 
         // decode plaintext_2
         let plaintext_2_decoded = decode_plaintext_2(&plaintext_2);
 
         if let Ok((c_r_2, id_cred_r, mac_2, ead_2)) = plaintext_2_decoded {
             let state = ProcessingM2 {
                 mac_2,
@@ -395,15 +396,15 @@
         Ok(state)
     } else {
         Err(EDHOCError::MacVerificationFailed)
     }
 }
 
 pub fn i_prepare_message_3(
-    state: &mut ProcessedM2,
+    state: &ProcessedM2,
     crypto: &mut impl CryptoTrait,
     cred_i: CredentialRPK,
     cred_transfer: CredentialTransfer,
     ead_3: &Option<EADItem>, // FIXME: make it a list of EADItem
 ) -> Result<(Completed, BufferMessage3, BytesHashLen), EDHOCError> {
     let mac_3 = compute_mac_3(
         crypto,
@@ -493,15 +494,15 @@
 }
 
 fn encode_message_1(
     method: u8,
     suites: &BytesSuites,
     suites_len: usize,
     g_x: &BytesP256ElemLen,
-    c_i: u8,
+    c_i: ConnId,
     ead_1: &Option<EADItem>,
 ) -> Result<BufferMessage1, EDHOCError> {
     let mut output = BufferMessage1::new();
     let mut raw_suites_len: usize = 0;
 
     output.content[0] = method; // CBOR unsigned int less than 24 is encoded verbatim
 
@@ -531,16 +532,17 @@
         }
     };
 
     output.content[1 + raw_suites_len] = CBOR_BYTE_STRING; // CBOR byte string magic number
     output.content[2 + raw_suites_len] = P256_ELEM_LEN as u8; // length of the byte string
     output.content[3 + raw_suites_len..3 + raw_suites_len + P256_ELEM_LEN]
         .copy_from_slice(&g_x[..]);
-    output.content[3 + raw_suites_len + P256_ELEM_LEN] = c_i;
-    output.len = 3 + raw_suites_len + P256_ELEM_LEN + 1;
+    let c_i = c_i.as_slice();
+    output.len = 3 + raw_suites_len + P256_ELEM_LEN + c_i.len();
+    output.content[3 + raw_suites_len + P256_ELEM_LEN..][..c_i.len()].copy_from_slice(c_i);
 
     if let Some(ead_1) = ead_1 {
         match encode_ead_item(ead_1) {
             Ok(ead_1) => output
                 .extend_from_slice(ead_1.as_slice())
                 .and(Ok(output))
                 .or(Err(EDHOCError::EadTooLongError)),
@@ -753,27 +755,28 @@
     let enc_structure = encode_enc_structure(th_3);
 
     crypto.aes_ccm_decrypt_tag_8(&k_3, &iv_3, &enc_structure, &ciphertext_3)
 }
 
 // output must hold id_cred.len() + cred.len()
 fn encode_kdf_context(
-    c_r: Option<u8>, // only present for MAC_2
+    c_r: Option<ConnId>, // only present for MAC_2
     id_cred: &BytesIdCred,
     th: &BytesHashLen,
     cred: &[u8],
     ead: &Option<EADItem>,
 ) -> (BytesMaxContextBuffer, usize) {
     // encode context in line
     // assumes ID_CRED_R and CRED_R are already CBOR-encoded (and also EAD)
     let mut output: BytesMaxContextBuffer = [0x00; MAX_KDF_CONTEXT_LEN];
 
     let mut output_len = if let Some(c_r) = c_r {
-        output[0] = c_r;
-        1 // size of u8
+        let c_r = c_r.as_slice();
+        output[..c_r.len()].copy_from_slice(c_r);
+        c_r.len()
     } else {
         0 // no u8 encoded
     };
     output[output_len..output_len + id_cred.len()].copy_from_slice(&id_cred[..]);
     output[output_len + id_cred.len()] = CBOR_BYTE_STRING;
     output[output_len + id_cred.len() + 1] = SHA256_DIGEST_LEN as u8;
     output[output_len + id_cred.len() + 2..output_len + id_cred.len() + 2 + th.len()]
@@ -820,15 +823,15 @@
     output[..MAC_LENGTH_3].copy_from_slice(&output_buf[..MAC_LENGTH_3]);
     output
 }
 
 fn compute_mac_2(
     crypto: &mut impl CryptoTrait,
     prk_3e2m: &BytesHashLen,
-    c_r: u8,
+    c_r: ConnId,
     id_cred_r: &BytesIdCred,
     cred_r: &[u8],
     th_2: &BytesHashLen,
     ead_2: &Option<EADItem>,
 ) -> BytesMac2 {
     // compute MAC_2
     let (context, context_len) = encode_kdf_context(Some(c_r), id_cred_r, th_2, cred_r, ead_2);
@@ -839,32 +842,33 @@
         &edhoc_kdf(crypto, prk_3e2m, 2_u8, &context, context_len, MAC_LENGTH_2)[..MAC_LENGTH_2],
     );
 
     mac_2
 }
 
 fn encode_plaintext_2(
-    c_r: u8,
+    c_r: ConnId,
     id_cred_r: &IdCred,
     mac_2: &BytesMac2,
     ead_2: &Option<EADItem>,
 ) -> Result<BufferPlaintext2, EDHOCError> {
     let mut plaintext_2: BufferPlaintext2 = BufferPlaintext2::new();
-    plaintext_2.content[0] = c_r;
+    let c_r = c_r.as_slice();
+    plaintext_2.content[..c_r.len()].copy_from_slice(c_r);
 
     let offset_cred = match id_cred_r {
         IdCred::CompactKid(kid) => {
-            plaintext_2.content[1] = *kid;
-            2
+            plaintext_2.content[c_r.len()] = *kid;
+            c_r.len() + 1
         }
         IdCred::FullCredential(cred) => {
-            plaintext_2.content[1] = CBOR_BYTE_STRING;
-            plaintext_2.content[2] = cred.len() as u8;
-            plaintext_2.content[3..3 + cred.len()].copy_from_slice(cred);
-            3 + cred.len()
+            plaintext_2.content[c_r.len()] = CBOR_BYTE_STRING;
+            plaintext_2.content[c_r.len() + 1] = cred.len() as u8;
+            plaintext_2.content[c_r.len() + 2..][..cred.len()].copy_from_slice(cred);
+            c_r.len() + 2 + cred.len()
         }
     };
 
     plaintext_2.content[offset_cred] = CBOR_MAJOR_BYTE_STRING | MAC_LENGTH_2 as u8;
     plaintext_2.content[1 + offset_cred..1 + offset_cred + mac_2.len()].copy_from_slice(&mac_2[..]);
     plaintext_2.len = 1 + offset_cred + mac_2.len();
 
@@ -884,15 +888,15 @@
 /// Apply the XOR base encryption for ciphertext_2 in place. This will decrypt (or decrypt) the bytes
 /// in the ciphertext_2 argument (which may alternatively contain plaintext), returning the cipher
 /// (or plain-)text.
 fn encrypt_decrypt_ciphertext_2(
     crypto: &mut impl CryptoTrait,
     prk_2e: &BytesHashLen,
     th_2: &BytesHashLen,
-    mut ciphertext_2: BufferCiphertext2,
+    ciphertext_2: &BufferCiphertext2,
 ) -> BufferCiphertext2 {
     // convert the transcript hash th_2 to BytesMaxContextBuffer type
     let mut th_2_context: BytesMaxContextBuffer = [0x00; MAX_KDF_CONTEXT_LEN];
     th_2_context[..th_2.len()].copy_from_slice(&th_2[..]);
 
     // KEYSTREAM_2 = EDHOC-KDF( PRK_2e,   0, TH_2,      plaintext_length )
     let keystream_2 = edhoc_kdf(
@@ -900,19 +904,21 @@
         prk_2e,
         0u8,
         &th_2_context,
         SHA256_DIGEST_LEN,
         ciphertext_2.len,
     );
 
+    let mut result = BufferCiphertext2::default();
     for i in 0..ciphertext_2.len {
-        ciphertext_2.content[i] ^= keystream_2[i];
+        result.content[i] = ciphertext_2.content[i] ^ keystream_2[i];
     }
+    result.len = ciphertext_2.len;
 
-    ciphertext_2
+    result
 }
 
 fn compute_salt_4e3m(
     crypto: &mut impl CryptoTrait,
     prk_3e2m: &BytesHashLen,
     th_3: &BytesHashLen,
 ) -> BytesHashLen {
@@ -1000,25 +1006,25 @@
     // test vectors (TV)
 
     // message_1 (first_time)
     const METHOD_TV_FIRST_TIME: u8 = 0x03;
     const SUITES_I_TV_FIRST_TIME: BytesSuites = hex!("060000000000000000");
     const G_X_TV_FIRST_TIME: BytesP256ElemLen =
         hex!("741a13d7ba048fbb615e94386aa3b61bea5b3d8f65f32620b749bee8d278efa9");
-    const C_I_TV_FIRST_TIME: u8 = 0x0e;
+    const C_I_TV_FIRST_TIME: ConnId = ConnId::from_int_raw(0x0e);
     const MESSAGE_1_TV_FIRST_TIME: &str =
         "03065820741a13d7ba048fbb615e94386aa3b61bea5b3d8f65f32620b749bee8d278efa90e";
 
     // message_1 (second time)
     const METHOD_TV: u8 = 0x03;
     // manually modified test vector to include a single supported cipher suite
     const SUITES_I_TV: BytesSuites = hex!("060200000000000000");
     const G_X_TV: BytesP256ElemLen =
         hex!("8af6f430ebe18d34184017a9a11bf511c8dff8f834730b96c1b7c8dbca2fc3b6");
-    const C_I_TV: u8 = 0x37;
+    const C_I_TV: ConnId = ConnId::from_int_raw(0x37);
     const MESSAGE_1_TV: &str =
         "0382060258208af6f430ebe18d34184017a9a11bf511c8dff8f834730b96c1b7c8dbca2fc3b637";
     // below are a few truncated messages for the purpose of testing cipher suites
     // message with one cipher suite (23..=255)
     const MESSAGE_1_TV_SUITE_ONLY_A: &str = "031818";
     // message with an array having two cipher suites with small values (0..=23)
     const MESSAGE_1_TV_SUITE_ONLY_B: &str = "03820201";
@@ -1033,15 +1039,15 @@
         "0382060258208af6f430ebe18d34184017a9a11bf511c8dff8f834730b96c1b7c8dbca2fc3b63701";
     const MESSAGE_1_WITH_DUMMY_EAD_TV: &str =
         "0382060258208af6f430ebe18d34184017a9a11bf511c8dff8f834730b96c1b7c8dbca2fc3b63701cccccc";
     const MESSAGE_1_WITH_DUMMY_CRITICAL_EAD_TV: &str =
         "0382060258208af6f430ebe18d34184017a9a11bf511c8dff8f834730b96c1b7c8dbca2fc3b63720cccccc";
     const G_Y_TV: BytesP256ElemLen =
         hex!("419701d7f00a26c2dc587a36dd752549f33763c893422c8ea0f955a13a4ff5d5");
-    const C_R_TV: u8 = 0x27;
+    const C_R_TV: ConnId = ConnId::from_int_raw(0x27);
     const MESSAGE_2_TV: &str = "582b419701d7f00a26c2dc587a36dd752549f33763c893422c8ea0f955a13a4ff5d59862a1eef9e0e7e1886fcd";
     const CIPHERTEXT_2_TV: &str = "9862a1eef9e0e7e1886fcd";
     const H_MESSAGE_1_TV: BytesHashLen =
         hex!("ca02cabda5a8902749b42f711050bb4dbd52153e87527594b39f50cdf019888c");
     const TH_2_TV: BytesHashLen =
         hex!("356efd53771425e008f3fe3a86c83ff4c6b16e57028ff39d5236c182b202084b");
     const TH_3_TV: BytesHashLen =
@@ -1413,25 +1419,25 @@
         let plaintext_2_tv = BufferPlaintext2::from_hex(PLAINTEXT_2_TV);
         let ciphertext_2_tv = BufferPlaintext2::from_hex(CIPHERTEXT_2_TV);
         // test decryption
         let plaintext_2 = encrypt_decrypt_ciphertext_2(
             &mut default_crypto(),
             &PRK_2E_TV,
             &TH_2_TV,
-            ciphertext_2_tv,
+            &ciphertext_2_tv,
         );
 
         assert_eq!(plaintext_2.len, PLAINTEXT_2_LEN_TV);
         for i in 0..PLAINTEXT_2_LEN_TV {
             assert_eq!(plaintext_2.content[i], plaintext_2_tv.content[i]);
         }
 
         // test encryption
         let ciphertext_2 =
-            encrypt_decrypt_ciphertext_2(&mut default_crypto(), &PRK_2E_TV, &TH_2_TV, plaintext_2);
+            encrypt_decrypt_ciphertext_2(&mut default_crypto(), &PRK_2E_TV, &TH_2_TV, &plaintext_2);
 
         assert_eq!(ciphertext_2.len, CIPHERTEXT_2_LEN_TV);
         for i in 0..CIPHERTEXT_2_LEN_TV {
             assert_eq!(ciphertext_2.content[i], ciphertext_2_tv.content[i]);
         }
     }
```

### Comparing `lakers_python-0.2.1/lib/src/lib.rs` & `lakers_python-0.3.0/lib/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-//! Implementation of [EDHOC] (Ephemeral Diffie-Hellman Over COSE), a lightweight authenticated key
+//! Implementation of [EDHOC] (Ephemeral Diffie-Hellman Over COSE, RFC9528), a lightweight authenticated key
 //! exchange for the Internet of Things.
 //!
 //! The crate provides a high-level interface through the [EdhocInitiator] and the [EdhocResponder]
 //! structs. Both these wrap the lower level [State] struct that is mainly used through internal
 //! functions in the `edhoc` module. This separation is relevant because the lower level tools are
 //! subject of ongoing formal verification, whereas the high-level interfaces aim for good
 //! usability.
 //!
 //! Both [EdhocInitiator] and [EdhocResponder] are used in a type stated way. Following the EDHOC
 //! protocol, they generate (or process) messages, progressively provide more information about
 //! their peer, and on eventually devolve into an [EdhocInitiatorDone] and [EdhocResponderDone],
 //! respectively, through which the EDHOC key material can be obtained.
 //!
-//! [EDHOC]: https://datatracker.ietf.org/doc/draft-ietf-lake-edhoc/
+//! [EDHOC]: https://datatracker.ietf.org/doc/html/rfc9528
 #![cfg_attr(not(test), no_std)]
 
 pub use {lakers_shared::Crypto as CryptoTrait, lakers_shared::*};
 
-#[cfg(any(feature = "ead-none", feature = "ead-authz"))]
-pub use lakers_ead::*;
+#[cfg(all(feature = "ead-authz", test))]
+pub use lakers_ead_authz::*;
 
 mod edhoc;
 pub use edhoc::*;
 
 // TODO: clean these structs and remove the cred_x whre they are not needed anymore
 /// Starting point for performing EDHOC in the role of the Initiator.
 #[derive(Debug)]
@@ -103,34 +103,42 @@
             crypto,
         }
     }
 
     pub fn process_message_1(
         mut self,
         message_1: &BufferMessage1,
-    ) -> Result<(EdhocResponderProcessedM1<'a, Crypto>, Option<EADItem>), EDHOCError> {
-        let (state, ead_1) = r_process_message_1(&self.state, &mut self.crypto, message_1)?;
+    ) -> Result<
+        (
+            EdhocResponderProcessedM1<'a, Crypto>,
+            ConnId,
+            Option<EADItem>,
+        ),
+        EDHOCError,
+    > {
+        let (state, c_i, ead_1) = r_process_message_1(&self.state, &mut self.crypto, message_1)?;
 
         Ok((
             EdhocResponderProcessedM1 {
                 state,
                 r: self.r,
                 cred_r: self.cred_r,
                 crypto: self.crypto,
             },
+            c_i,
             ead_1,
         ))
     }
 }
 
 impl<'a, Crypto: CryptoTrait> EdhocResponderProcessedM1<'a, Crypto> {
     pub fn prepare_message_2(
         mut self,
         cred_transfer: CredentialTransfer,
-        c_r: Option<u8>,
+        c_r: Option<ConnId>,
         ead_2: &Option<EADItem>,
     ) -> Result<(EdhocResponderWaitM3<Crypto>, BufferMessage2), EDHOCError> {
         let c_r = match c_r {
             Some(c_r) => c_r,
             None => generate_connection_identifier_cbor(&mut self.crypto),
         };
 
@@ -249,15 +257,15 @@
             },
             crypto,
         }
     }
 
     pub fn prepare_message_1(
         mut self,
-        c_i: Option<u8>,
+        c_i: Option<ConnId>,
         ead_1: &Option<EADItem>,
     ) -> Result<(EdhocInitiatorWaitM2<Crypto>, EdhocMessageBuffer), EDHOCError> {
         let c_i = match c_i {
             Some(c_i) => c_i,
             None => generate_connection_identifier_cbor(&mut self.crypto),
         };
 
@@ -285,15 +293,15 @@
 impl<'a, Crypto: CryptoTrait> EdhocInitiatorWaitM2<Crypto> {
     pub fn parse_message_2(
         mut self,
         message_2: &'a BufferMessage2,
     ) -> Result<
         (
             EdhocInitiatorProcessingM2<Crypto>,
-            u8,
+            ConnId,
             CredentialRPK,
             Option<EADItem>,
         ),
         EDHOCError,
     > {
         match i_parse_message_2(&self.state, &mut self.crypto, message_2) {
             Ok((state, c_r, id_cred_r, ead_2)) => Ok((
@@ -395,37 +403,37 @@
             &mut self.crypto,
             &context_buf,
             context.len(),
         )
     }
 }
 
-pub fn generate_connection_identifier_cbor<Crypto: CryptoTrait>(crypto: &mut Crypto) -> u8 {
+pub fn generate_connection_identifier_cbor<Crypto: CryptoTrait>(crypto: &mut Crypto) -> ConnId {
     let c_i = generate_connection_identifier(crypto);
-    if c_i >= 0 && c_i <= 23 {
+    ConnId::from_int_raw(if c_i >= 0 && c_i <= 23 {
         c_i as u8 // verbatim encoding of single byte integer
     } else if c_i < 0 && c_i >= -24 {
         // negative single byte integer encoding
         CBOR_NEG_INT_1BYTE_START - 1 + c_i.unsigned_abs()
     } else {
         0
-    }
+    })
 }
 
 /// generates an identifier that can be serialized as a single CBOR integer, i.e. -24 <= x <= 23
 pub fn generate_connection_identifier<Crypto: CryptoTrait>(crypto: &mut Crypto) -> i8 {
     let mut conn_id = crypto.get_random_byte() as i8;
     while conn_id < -24 || conn_id > 23 {
         conn_id = crypto.get_random_byte() as i8;
     }
     conn_id
 }
 
 // Implements auth credential checking according to draft-tiloca-lake-implem-cons
-pub fn credential_check_or_fetch<'a>(
+pub fn credential_check_or_fetch(
     cred_expected: Option<CredentialRPK>,
     id_cred_received: CredentialRPK,
 ) -> Result<CredentialRPK, EDHOCError> {
     // Processing of auth credentials according to draft-tiloca-lake-implem-cons
     // Comments tagged with a number refer to steps in Section 4.3.1. of draft-tiloca-lake-implem-cons
     if let Some(cred_expected) = cred_expected {
         // 1. Does ID_CRED_X point to a stored authentication credential? YES
@@ -442,15 +450,15 @@
 
         // Continue by considering CRED_X as the authentication credential of the other peer.
         // IMPL: ready to proceed, including process ead_2
 
         if credentials_match {
             Ok(cred_expected)
         } else {
-            Err(EDHOCError::UnknownPeer)
+            Err(EDHOCError::UnexpectedCredential)
         }
     } else {
         // 1. Does ID_CRED_X point to a stored authentication credential? NO
         // IMPL: cred_i_expected provided by application is None
         //       id_cred must be a full credential
         // 3. Is the trust model Pre-knowledge-only? NO (hardcoded to NO for now)
         // 4. Is the trust model Pre-knowledge + TOFU? YES (hardcoded to YES for now)
@@ -563,15 +571,15 @@
 
         // ---- begin initiator handling
         // if needed: prepare ead_1
         let (initiator, message_1) = initiator.prepare_message_1(None, &None).unwrap();
         // ---- end initiator handling
 
         // ---- begin responder handling
-        let (responder, _ead_1) = responder.process_message_1(&message_1).unwrap();
+        let (responder, _c_i, _ead_1) = responder.process_message_1(&message_1).unwrap();
         // if ead_1: process ead_1
         // if needed: prepare ead_2
         let (responder, message_2) = responder
             .prepare_message_2(CredentialTransfer::ByReference, None, &None)
             .unwrap();
         // ---- end responder handling
 
@@ -603,34 +611,32 @@
         let r_oscore_secret = responder.edhoc_exporter(0u8, &[], 16); // label is 0
         let r_oscore_salt = responder.edhoc_exporter(1u8, &[], 8); // label is 1
 
         assert_eq!(i_oscore_secret, r_oscore_secret);
         assert_eq!(i_oscore_salt, r_oscore_salt);
 
         // test key update with context from draft-ietf-lake-traces
-        let i_prk_out_new = initiator.edhoc_key_update(&[
+        let context = &[
             0xa0, 0x11, 0x58, 0xfd, 0xb8, 0x20, 0x89, 0x0c, 0xd6, 0xbe, 0x16, 0x96, 0x02, 0xb8,
             0xbc, 0xea,
-        ]);
-        let r_prk_out_new = responder.edhoc_key_update(&[
-            0xa0, 0x11, 0x58, 0xfd, 0xb8, 0x20, 0x89, 0x0c, 0xd6, 0xbe, 0x16, 0x96, 0x02, 0xb8,
-            0xbc, 0xea,
-        ]);
+        ];
+        let i_prk_out_new = initiator.edhoc_key_update(context);
+        let r_prk_out_new = responder.edhoc_key_update(context);
 
         assert_eq!(i_prk_out_new, r_prk_out_new);
     }
 }
 
 #[cfg(feature = "test-ead-authz")]
 #[cfg(test)]
 mod test_authz {
     use super::*;
     use hexlit::hex;
     use lakers_crypto::default_crypto;
-    use lakers_ead::*;
+    use lakers_ead_authz::*;
     use test_vectors_common::*;
 
     // U
     const ID_U_TV: &[u8] = &hex!("a104412b");
 
     // V -- nothing to do, will reuse CRED_R from above to act as CRED_V
 
@@ -642,14 +648,22 @@
 
     // TODO: have a setup_test function that prepares the common objects for the ead tests
     #[test]
     fn test_handshake_authz() {
         let cred_i = CredentialRPK::new(CRED_I.try_into().unwrap()).unwrap();
         let cred_r = CredentialRPK::new(CRED_R.try_into().unwrap()).unwrap();
 
+        let mock_fetch_cred_i = |id_cred_i: CredentialRPK| -> Result<CredentialRPK, EDHOCError> {
+            if id_cred_i.kid == cred_i.kid {
+                Ok(cred_i.clone())
+            } else {
+                Err(EDHOCError::UnexpectedCredential)
+            }
+        };
+
         // ==== initialize edhoc ====
         let mut initiator = EdhocInitiator::new(default_crypto());
         let responder = EdhocResponder::new(default_crypto(), R, cred_r);
 
         // ==== initialize ead-authz ====
         let device = ZeroTouchDevice::new(
             ID_U_TV.try_into().unwrap(),
@@ -671,15 +685,15 @@
             &mut default_crypto(),
             initiator.compute_ephemeral_secret(&device.g_w),
             initiator.selected_cipher_suite(),
         );
         let (initiator, message_1) = initiator.prepare_message_1(None, &Some(ead_1)).unwrap();
         device.set_h_message_1(initiator.state.h_message_1.clone());
 
-        let (responder, ead_1) = responder.process_message_1(&message_1).unwrap();
+        let (responder, _c_i, ead_1) = responder.process_message_1(&message_1).unwrap();
         let ead_2 = if let Some(ead_1) = ead_1 {
             let (authenticator, _loc_w, voucher_request) =
                 authenticator.process_ead_1(&ead_1, &message_1).unwrap();
 
             // the line below mocks a request to the server: let voucher_response = auth_client.post(loc_w, voucher_request)?
             let voucher_response = server
                 .handle_voucher_request(&mut default_crypto(), &voucher_request)
@@ -704,14 +718,18 @@
         let initiator = initiator.verify_message_2(I, cred_i, valid_cred_r).unwrap();
 
         let (mut _initiator, message_3, i_prk_out) = initiator
             .prepare_message_3(CredentialTransfer::ByReference, &None)
             .unwrap();
 
         let (responder, id_cred_i, _ead_3) = responder.parse_message_3(&message_3).unwrap();
-        let valid_cred_i = credential_check_or_fetch(Some(cred_i), id_cred_i).unwrap();
+        let valid_cred_i = if id_cred_i.reference_only() {
+            mock_fetch_cred_i(id_cred_i).unwrap()
+        } else {
+            id_cred_i
+        };
         let (mut _responder, r_prk_out) = responder.verify_message_3(valid_cred_i).unwrap();
 
         // check that prk_out is equal at initiator and responder side
         assert_eq!(i_prk_out, r_prk_out);
     }
 }
```

### Comparing `lakers_python-0.2.1/README.md` & `lakers_python-0.3.0/lib/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,64 @@
-# lakers: EDHOC implemented in Rust
+# lakers &emsp; [![CI status]][actions] [![Latest Version]][crates.io] [![API Documentation]][docs.rs]
 
-[![Build and test](https://github.com/openwsn-berkeley/lakers/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/openwsn-berkeley/lakers/actions/workflows/build-and-test.yml)
+[CI status]: https://github.com/openwsn-berkeley/lakers/actions/workflows/build-and-test.yml/badge.svg
+[actions]: https://github.com/openwsn-berkeley/lakers/actions/workflows/build-and-test.yml
+[Latest Version]: https://img.shields.io/crates/v/lakers.svg
+[crates.io]: https://crates.io/crates/lakers
+[API Documentation]: https://docs.rs/lakers/badge.svg
+[docs.rs]: https://docs.rs/lakers
 
-An implementation of [EDHOC](https://datatracker.ietf.org/doc/draft-ietf-lake-edhoc/) in Rust:
-- up-to-date with the [latest draft version (23)](https://datatracker.ietf.org/doc/draft-ietf-lake-edhoc/23/)
+An implementation of [EDHOC (RFC 9528)](https://datatracker.ietf.org/doc/html/rfc9528) in Rust.
+
+# What is EDHOC?
+
+Ephemeral Diffie-Hellman Over COSE (EDHOC) is a new IETF standard that provides a [very lightweight](https://hal.science/hal-04382397/document) authenticated key exchange, ideal for usage in constrained scenarios, such as in Internet of Things environments.
+
+# EDHOC Features
+- lightweight: full authenticated key exchange in as few as 101 bytes
+- secure: mutual authentication, forward secrecy, and identity protection
+- transport-agnostic: can be used on scenarios with or without IP connectivity; a common way to transport EDHOC is [over reliable CoAP](https://www.rfc-editor.org/rfc/rfc9528.html#coap)
+- code re-use: achieved due to re-using technologies common in IoT scenarios, such as COSE, CBOR, and CoAP
+- finally, a main use case of EDHOC is to establish an [OSCORE](https://datatracker.ietf.org/doc/rfc8613/) security context
+
+
+# lakers features
+
+- easy to use, typestated API for Initiator and Responder
 - microcontroller-optimized: `no_std`, no heap allocations, zero-dependencies (other than crypto backends)
 - configurable crypto backends
 - bindings for [C](https://github.com/openwsn-berkeley/lakers/releases/) and [Python](https://pypi.org/project/lakers-python/)
 - support for EDHOC extensions, including [zero-touch authorization](https://datatracker.ietf.org/doc/draft-ietf-lake-authz/)
 
 It currently supports authentication mode STAT-STAT and Cipher Suite 2 (AES-CCM-16-64-128, SHA-256, 8, P-256, ES256, AES-CCM-16-64-128, SHA-256).
 
+# Getting started
+
+To use `lakers` in your Rust project, add it to your Cargo.toml using `cargo add lakers`.
+
 Here's a quick look at the API for the Initiator role (for the Responder role, and more details, check the examples or the unit tests):
 ```rust
+// perform the handshake
 let initiator = EdhocInitiator::new(default_crypto());
 
 let (initiator, message_1) = initiator.prepare_message_1(None, &None)?; // c_i and ead_1 are set to None
 
 let (initiator, _c_r, id_cred_r, _ead_2) = initiator.parse_message_2(&message_2)?;
 let valid_cred_r = credential_check_or_fetch(Some(CRED_R), id_cred_r)?; // CRED_R contains Responder's public key
 let initiator = initiator.verify_message_2(I, cred_i, valid_cred_r)?; // I is Initiator's private key
 
 let (mut initiator, message_3, i_prk_out) = initiator.prepare_message_3(CredentialTransfer::ByReference, &None)?; // no ead_3
-```
 
-## Installation
+// derive a secret to use with OSCORE
+let oscore_secret = initiator.edhoc_exporter(0u8, &[], 16); // label is 0
 
-To use `lakers` in your Rust project, simply add it to your Cargo.toml: `lakers = "0.5.1"` (check for the [latest version here](https://crates.io/crates/lakers)).
+// update the prk_out key (context taken from draft-ietf-lake-traces)
+let context = &[0xa0, 0x11, 0x58, 0xfd, 0xb8, 0x20, 0x89, 0x0c, 0xd6, 0xbe, 0x16, 0x96, 0x02, 0xb8, 0xbc, 0xea];
+let prk_out_new = initiator.edhoc_key_update(context);
+```
 
 ### C API
 C-compatible static libraries and headers are available for download in [the releases page](https://github.com/openwsn-berkeley/lakers/releases).
 
 ### Python API
 `lakers-python` is [available on PyPI](https://pypi.org/project/lakers-python/), to install it run `pip install lakers-python`.
 
@@ -85,13 +113,13 @@
 1. run one of the commands above, but use the command `embed` in place of `build`. For example: `cargo embed --target="thumbv7em-none-eabihf"`
 
 ## Directory structure
 This library is structured as a [cargo workspace](https://doc.rust-lang.org/book/ch14-03-cargo-workspaces.html).
 Its main members are:
 
 - `lib`: The main library providing the EDHOC implementation.
-- `crypto`: Diferent cryptographic backends (e.g. psa, cryptocell310, hacspec).
+- `crypto`: Diferent cryptographic backends (e.g. psa, cryptocell310, rustcrypto).
 - `ead`: Implementation of extensions to EDHOC via the External Authorization Data (EAD) field.
 - `shared`: Defines shared structs and modules used throughout the workspace members.
 - `lakers-c`: Provides a foreign function interface that enables using `lakers` from C code.
 - `lakers-python`: API for using `lakers` in Python.
 - `examples`: Example applications that demonstrate how to use the library.
```

### Comparing `lakers_python-0.2.1/crypto/Cargo.toml` & `lakers_python-0.3.0/crypto/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -7,34 +7,30 @@
 description = "EDHOC crypto library dispatch crate"
 repository.workspace = true
 readme.workspace = true
 
 [dependencies]
 lakers-shared = { package = "lakers-shared", path = "../shared", default-features = false }
 
-# hacspec
-# lakers-crypto-hacspec = { workspace = true, optional = true }
-
-# cc2538 hardware accelerated
-lakers-crypto-cc2538 = { workspace = true, optional = true }
-
 # psa
 lakers-crypto-psa = { workspace = true, default-features = false, optional = true }
 
 # cryptocell for nrf52840
 lakers-crypto-cryptocell310 = { workspace = true, optional = true }
 
 # software implementations from rustcrypto
 lakers-crypto-rustcrypto = { workspace = true, optional = true }
 rand_core = { version = "0.6.4", optional = true, default-features = false }
 
+[dev-dependencies]
+hexlit = "0.5.3"
+rstest = "0.11.0"
+
 [features]
 default = [  ]
-# hacspec = [ "lakers-crypto-hacspec" ]
-cc2538 = [ "lakers-crypto-cc2538" ]
 psa = [ "lakers-crypto-psa" ]
 psa-baremetal = [ "psa", "lakers-crypto-psa/baremetal" ]
 cryptocell310 = [ "lakers-crypto-cryptocell310" ]
 # This requires std because we need to conjure randomness from thin air;
 # embedded systems can still use rustcrypto but need to provide a crypto from
 # lakers-crypto-rustcrypto on their own, and combine it with an entropy choice
 # of their avail.
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/cbindgen.toml` & `lakers_python-0.3.0/ead/lakers-ead-authz/cbindgen.toml`

 * *Files 26% similar despite different names*

```diff
@@ -8,9 +8,10 @@
  *  WARNING: This file is automatically generated by cbindgen. Manual edits are likely to be lost.
  * ================================================================================================
  */"""
 include_guard = "LAKERS_EAD_AUTHZ_H"
 
 [export]
 include = [
+    "EadAuthzDevice",
     "ZeroTouchDevice", "ZeroTouchDeviceWaitEAD2", "ZeroTouchDeviceDone"
 ]
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/src/authenticator.rs` & `lakers_python-0.3.0/ead/lakers-ead-authz/src/authenticator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-use super::shared::*;
+use crate::consts::*;
+use crate::shared::*;
 use lakers_shared::*;
 
 #[derive(Debug, Default)]
 pub struct ZeroTouchAuthenticator;
 #[derive(Debug, Default)]
 pub struct ZeroTouchAuthenticatorWaitVoucherResp;
 
@@ -17,16 +18,16 @@
             EdhocMessageBuffer,
             EdhocMessageBuffer,
         ),
         EDHOCError,
     > {
         let opaque_state: Option<EdhocMessageBuffer> = None; // TODO: receive as parameter
 
-        if ead_1.label != EAD_ZEROCONF_LABEL || ead_1.value.is_none() {
-            return Err(EDHOCError::EADError);
+        if ead_1.label != EAD_AUTHZ_LABEL || ead_1.value.is_none() {
+            return Err(EDHOCError::EADUnprocessable);
         }
 
         let (loc_w, _enc_id) = parse_ead_1_value(&ead_1.value.unwrap())?;
         let voucher_request = encode_voucher_request(message_1, &opaque_state);
 
         Ok((
             ZeroTouchAuthenticatorWaitVoucherResp::default(),
@@ -40,15 +41,15 @@
     pub fn prepare_ead_2(
         &self,
         voucher_response: &EdhocMessageBuffer,
     ) -> Result<EADItem, EDHOCError> {
         let (_message_1, voucher, _opaque_state) = parse_voucher_response(&voucher_response)?;
 
         Ok(EADItem {
-            label: EAD_ZEROCONF_LABEL,
+            label: EAD_AUTHZ_LABEL,
             is_critical: true,
             value: Some(voucher[..].try_into().unwrap()),
         })
     }
 }
 
 pub fn encode_voucher_request(
@@ -88,15 +89,15 @@
     ),
     EDHOCError,
 > {
     let mut decoder = CBORDecoder::new(voucher_response.as_slice());
 
     let array_size = decoder.array()?;
     if !(2..=3).contains(&array_size) {
-        return Err(EDHOCError::EADError);
+        return Err(EDHOCError::EADUnprocessable);
     }
 
     let message_1: EdhocMessageBuffer = decoder.bytes()?.try_into().unwrap();
     let voucher: BytesEncodedVoucher = decoder
         .bytes_sized(ENCODED_VOUCHER_LEN)?
         .try_into()
         .unwrap();
@@ -134,15 +135,15 @@
             encode_voucher_request(&MESSAGE_1_WITH_EAD_TV.try_into().unwrap(), &None);
         assert_eq!(voucher_request.content, voucher_request_tv.content);
     }
 
     #[test]
     fn test_process_ead_1() {
         let ead_1 = EADItem {
-            label: EAD_ZEROCONF_LABEL,
+            label: EAD_AUTHZ_LABEL,
             is_critical: true,
             value: Some(EAD1_VALUE_TV.try_into().unwrap()),
         };
 
         let ead_authenticator = ZeroTouchAuthenticator::default();
         let res =
             ead_authenticator.process_ead_1(&ead_1, &MESSAGE_1_WITH_EAD_TV.try_into().unwrap());
@@ -169,15 +170,15 @@
         let ead_2_value_tv: EdhocMessageBuffer = EAD2_VALUE_TV.try_into().unwrap();
 
         let ead_authenticator = ZeroTouchAuthenticatorWaitVoucherResp::default();
 
         let ead_2 = ead_authenticator
             .prepare_ead_2(&voucher_response_tv)
             .unwrap();
-        assert_eq!(ead_2.label, EAD_ZEROCONF_LABEL);
+        assert_eq!(ead_2.label, EAD_AUTHZ_LABEL);
         assert_eq!(ead_2.is_critical, true);
         assert_eq!(ead_2.value.unwrap().content, ead_2_value_tv.content);
     }
 }
 
 #[cfg(test)]
 mod test_responder_stateless_operation {
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/src/device.rs` & `lakers_python-0.3.0/ead/lakers-ead-authz/src/device.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-use super::shared::*;
+use crate::consts::*;
+use crate::shared::*;
 use crate::ZeroTouchError;
 use lakers_shared::{Crypto as CryptoTrait, *};
 
 #[derive(Default, Debug)]
 #[repr(C)]
 pub struct ZeroTouchDevice {
     pub id_u: EdhocMessageBuffer, // identifier of the device (U), equivalent to ID_CRED_I in EDHOC
@@ -39,15 +40,15 @@
 
         // plaintext = (ID_U: bstr)
         let encoded_id_u = encode_id_u(&self.id_u);
         let enc_id = encrypt_enc_id(crypto, &prk, &encoded_id_u, ss);
         let value = Some(encode_ead_1_value(&self.loc_w, &enc_id));
 
         let ead_1 = EADItem {
-            label: EAD_ZEROCONF_LABEL,
+            label: EAD_AUTHZ_LABEL,
             is_critical: true,
             value,
         };
 
         (
             ZeroTouchDeviceWaitEAD2 {
                 prk,
@@ -65,15 +66,15 @@
 
     pub fn process_ead_2<Crypto: CryptoTrait>(
         &self,
         crypto: &mut Crypto,
         ead_2: EADItem,
         cred_v: &[u8],
     ) -> Result<ZeroTouchDeviceDone, ZeroTouchError> {
-        if ead_2.label != EAD_ZEROCONF_LABEL {
+        if ead_2.label != EAD_AUTHZ_LABEL {
             return Err(ZeroTouchError::InvalidEADLabel);
         }
         let Some(ead_2_value_buffer) = ead_2.value else {
             return Err(ZeroTouchError::EmptyEADValue);
         };
         let mut ead_2_value: BytesEncodedVoucher = Default::default();
         ead_2_value[..].copy_from_slice(&ead_2_value_buffer.content[..ENCODED_VOUCHER_LEN]);
@@ -176,15 +177,15 @@
             ID_U_TV.try_into().unwrap(),
             G_W_TV.try_into().unwrap(),
             LOC_W_TV.try_into().unwrap(),
         );
 
         let (_ead_device, ead_1) =
             ead_device.prepare_ead_1(&mut default_crypto(), G_XW_TV.try_into().unwrap(), SS_TV);
-        assert_eq!(ead_1.label, EAD_ZEROCONF_LABEL);
+        assert_eq!(ead_1.label, EAD_AUTHZ_LABEL);
         assert_eq!(ead_1.is_critical, true);
         assert_eq!(ead_1.value.unwrap().content, ead_1_value_tv.content);
     }
 
     #[test]
     fn test_verify_voucher() {
         let mut voucher_tv = VOUCHER_TV.try_into().unwrap();
@@ -212,15 +213,15 @@
         );
         assert_eq!(res, Err(ZeroTouchError::VoucherVerificationFailed));
     }
 
     #[test]
     fn test_process_ead_2() {
         let ead_2_tv = EADItem {
-            label: EAD_ZEROCONF_LABEL,
+            label: EAD_AUTHZ_LABEL,
             is_critical: true,
             value: Some(EAD2_VALUE_TV.try_into().unwrap()),
         };
 
         let ead_device = ZeroTouchDeviceWaitEAD2 {
             prk: PRK_TV.try_into().unwrap(),
             h_message_1: H_MESSAGE_1_TV.try_into().unwrap(),
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/src/lib.rs` & `lakers_python-0.3.0/ead/lakers-ead-authz/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 #[cfg(test)]
 mod test_vectors;
 
 pub use authenticator::{ZeroTouchAuthenticator, ZeroTouchAuthenticatorWaitVoucherResp};
 pub use device::{ZeroTouchDevice, ZeroTouchDeviceDone, ZeroTouchDeviceWaitEAD2};
 pub use server::{ZeroTouchServer, ZeroTouchServerUserAcl};
 
+pub mod consts {
+    pub const EAD_AUTHZ_LABEL: u8 = 0x1; // NOTE: in lake-authz-draft-01 it is still TBD1
+    pub const EAD_AUTHZ_INFO_K_1_LABEL: u8 = 0x0;
+    pub const EAD_AUTHZ_INFO_IV_1_LABEL: u8 = 0x1;
+    pub const EAD_AUTHZ_ENC_STRUCTURE_LEN: usize = 2 + 8 + 3;
+}
+
 #[derive(PartialEq, Debug)]
 #[repr(C)]
 pub enum ZeroTouchError {
     InvalidEADLabel,
     EmptyEADValue,
     VoucherVerificationFailed,
 }
@@ -88,10 +95,10 @@
 
         let (_authenticator, _loc_w, voucher_request) = authenticator
             .process_ead_1(&ead_1, &MESSAGE_1_WITH_EAD_TV.try_into().unwrap())
             .unwrap();
 
         let voucher_response =
             server.handle_voucher_request(&mut default_crypto(), &voucher_request);
-        assert_eq!(voucher_response.unwrap_err(), EDHOCError::EADError);
+        assert_eq!(voucher_response.unwrap_err(), EDHOCError::AccessDenied);
     }
 }
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/src/server.rs` & `lakers_python-0.3.0/ead/lakers-ead-authz/src/server.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use super::shared::*;
+use crate::shared::*;
 use lakers_shared::{Crypto as CryptoTrait, *};
 
 /// This server also stores an ACL
 #[derive(PartialEq, Debug, Copy, Clone)]
 pub struct ZeroTouchServer {
     w: BytesP256ElemLen,            // private key of the enrollment server (W)
     pub cred_v: EdhocMessageBuffer, // credential of the authenticator (V)
@@ -44,15 +44,15 @@
             message_1_buf[..message_1.len].copy_from_slice(message_1.as_slice());
             let h_message_1 = crypto.sha256_digest(&message_1_buf, message_1.len);
 
             let voucher = prepare_voucher(crypto, &h_message_1, &self.cred_v.as_slice(), &prk);
             let voucher_response = encode_voucher_response(&message_1, &voucher, &opaque_state);
             Ok(voucher_response)
         } else {
-            Err(EDHOCError::EADError)
+            Err(EDHOCError::AccessDenied)
         }
     }
 }
 
 /// This server can be used when the ACL is stored in the application layer
 #[derive(PartialEq, Debug, Copy, Clone)]
 pub struct ZeroTouchServerUserAcl {
@@ -103,15 +103,15 @@
 
 fn parse_voucher_request(
     vreq: &EdhocMessageBuffer,
 ) -> Result<(EdhocMessageBuffer, Option<EdhocMessageBuffer>), EDHOCError> {
     let mut decoder = CBORDecoder::new(vreq.as_slice());
     let array_size = decoder.array()?;
     if array_size != 1 && array_size != 2 {
-        return Err(EDHOCError::EADError);
+        return Err(EDHOCError::EADUnprocessable);
     }
 
     let message_1: EdhocMessageBuffer = decoder.bytes()?.try_into().unwrap();
 
     if array_size == 2 {
         let opaque_state: EdhocMessageBuffer = decoder.bytes()?.try_into().unwrap();
         Ok((message_1, Some(opaque_state)))
@@ -273,15 +273,15 @@
             Some(ACL_INVALID_TV.try_into().unwrap()),
         );
 
         let res = ead_server.handle_voucher_request(
             &mut default_crypto(),
             &VOUCHER_REQUEST_TV.try_into().unwrap(),
         );
-        assert_eq!(res.unwrap_err(), EDHOCError::EADError);
+        assert_eq!(res.unwrap_err(), EDHOCError::AccessDenied);
     }
 }
 
 #[cfg(test)]
 mod test_enrollment_server_acl_user {
     use super::*;
     use crate::test_vectors::*;
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/src/shared.rs` & `lakers_python-0.3.0/ead/lakers-ead-authz/src/shared.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use crate::consts::*;
 use lakers_shared::{Crypto as CryptoTrait, *};
 
 pub(crate) fn compute_prk<Crypto: CryptoTrait>(
     crypto: &mut Crypto,
     a: &BytesP256ElemLen,
     g_b: &BytesP256ElemLen,
 ) -> BytesHashLen {
@@ -38,27 +39,27 @@
     prk: &BytesHashLen,
 ) -> (BytesCcmKeyLen, BytesCcmIvLen) {
     // K_1 = EDHOC-Expand(PRK, info = (0, h'', AES_CCM_KEY_LEN), length)
     let mut k_1: BytesCcmKeyLen = [0x00; AES_CCM_KEY_LEN];
     let k_1_buf = edhoc_kdf_expand(
         crypto,
         prk,
-        EAD_ZEROCONF_INFO_K_1_LABEL,
+        EAD_AUTHZ_INFO_K_1_LABEL,
         &[0x00; MAX_KDF_CONTEXT_LEN],
         0,
         AES_CCM_KEY_LEN,
     );
     k_1[..].copy_from_slice(&k_1_buf[..AES_CCM_KEY_LEN]);
 
     // IV_1 = EDHOC-Expand(PRK, info = (1, h'', AES_CCM_IV_LEN), length)
     let mut iv_1: BytesCcmIvLen = [0x00; AES_CCM_IV_LEN];
     let iv_1_buf = edhoc_kdf_expand(
         crypto,
         prk,
-        EAD_ZEROCONF_INFO_IV_1_LABEL,
+        EAD_AUTHZ_INFO_IV_1_LABEL,
         &[0x00; MAX_KDF_CONTEXT_LEN],
         0,
         AES_CCM_IV_LEN,
     );
     iv_1[..].copy_from_slice(&iv_1_buf[..AES_CCM_IV_LEN]);
 
     (k_1, iv_1)
@@ -72,27 +73,26 @@
     let mut seq_decoder = CBORDecoder::new(voucher_info_seq);
     Ok((
         seq_decoder.str()?.try_into().unwrap(),
         seq_decoder.bytes()?.try_into().unwrap(),
     ))
 }
 
-pub(crate) fn encode_enc_structure(ss: u8) -> [u8; EAD_ZEROCONF_ENC_STRUCTURE_LEN] {
+pub(crate) fn encode_enc_structure(ss: u8) -> [u8; EAD_AUTHZ_ENC_STRUCTURE_LEN] {
     let mut encrypt0: Bytes8 = [0x00; 8];
     encrypt0[0] = 0x45u8; // 'E'
     encrypt0[1] = 0x6eu8; // 'n'
     encrypt0[2] = 0x63u8; // 'c'
     encrypt0[3] = 0x72u8; // 'r'
     encrypt0[4] = 0x79u8; // 'y'
     encrypt0[5] = 0x70u8; // 'p'
     encrypt0[6] = 0x74u8; // 't'
     encrypt0[7] = 0x30u8; // '0'
 
-    let mut enc_structure: [u8; EAD_ZEROCONF_ENC_STRUCTURE_LEN] =
-        [0x00; EAD_ZEROCONF_ENC_STRUCTURE_LEN];
+    let mut enc_structure: [u8; EAD_AUTHZ_ENC_STRUCTURE_LEN] = [0x00; EAD_AUTHZ_ENC_STRUCTURE_LEN];
 
     // encode Enc_structure from rfc9052 Section 5.3
     enc_structure[0] = CBOR_MAJOR_ARRAY | 3 as u8; // 3 is the fixed number of elements in the array
     enc_structure[1] = CBOR_MAJOR_TEXT_STRING | encrypt0.len() as u8;
     enc_structure[2..2 + encrypt0.len()].copy_from_slice(&encrypt0[..]);
     enc_structure[encrypt0.len() + 2] = CBOR_MAJOR_BYTE_STRING | 0x00 as u8; // 0 for zero-length byte string (empty Header)
     enc_structure[encrypt0.len() + 3] = CBOR_MAJOR_BYTE_STRING | 0x01 as u8; // 1 for the `ss` value
```

### Comparing `lakers_python-0.2.1/ead/lakers-ead-authz/src/test_vectors.rs` & `lakers_python-0.3.0/ead/lakers-ead-authz/src/test_vectors.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/shared/Cargo.toml` & `lakers_python-0.3.0/shared/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 edition = "2021"
 authors = ["Mališa Vučinić <malisa.vucinic@inria.fr>"]
 license.workspace = true
 description = "EDHOC crypto library constants crate"
 repository.workspace = true
 # It's implied, but still better for consistency to have it explicit.
 readme.workspace = true
+keywords.workspace = true
+categories.workspace = true
 
 [dependencies]
 pyo3 = { version = "0.20.2", features = ["extension-module"], optional = true }
 
 [dev-dependencies]
 hexlit = "0.5.3"
```

### Comparing `lakers_python-0.2.1/shared/cbindgen.toml` & `lakers_python-0.3.0/shared/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/shared/src/cred.rs` & `lakers_python-0.3.0/shared/src/cred.rs`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     }
 
     pub fn get_id_cred(&self) -> BytesIdCred {
         [0xa1, 0x04, 0x41, self.kid] // cbor map = {4: kid}
     }
 
     fn parse(cred: &[u8]) -> Result<(BytesP256ElemLen, u8), EDHOCError> {
-        // NOTE: this routine is only guaranteed to work with credentials from lake-traces
+        // NOTE: this routine is only guaranteed to work with credentials from RFC9529
         const CCS_PREFIX_LEN: usize = 3;
         const CNF_AND_COSE_KEY_PREFIX_LEN: usize = 8;
         const COSE_KEY_FIRST_ITEMS_LEN: usize = 6;
 
         if cred.len()
             < 3 + CCS_PREFIX_LEN
                 + 1
```

### Comparing `lakers_python-0.2.1/shared/src/crypto.rs` & `lakers_python-0.3.0/shared/src/crypto.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/shared/src/lib.rs` & `lakers_python-0.3.0/shared/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 //       then the crate will be no_std
 #![cfg_attr(not(feature = "python-bindings"), no_std)]
 
 pub use cbor_decoder::*;
 pub use edhoc_parser::*;
 pub use helpers::*;
 
+use core::num::NonZeroI16;
+
 mod crypto;
 pub use crypto::Crypto;
 
 mod cred;
 pub use cred::*;
 
 #[cfg(feature = "python-bindings")]
@@ -64,18 +66,14 @@
 				            1 + MAX_KDF_LABEL_LEN +     // label <24 bytes as tstr
 						    1 + MAX_KDF_CONTEXT_LEN +   // context <24 bytes as bstr
 						    1; // length as u8
 
 pub const ENC_STRUCTURE_LEN: usize = 8 + 5 + SHA256_DIGEST_LEN; // 8 for ENCRYPT0
 
 pub const MAX_EAD_SIZE_LEN: usize = 64;
-pub const EAD_ZEROCONF_LABEL: u8 = 0x1; // NOTE: in lake-authz-draft-02 it is still TBD1
-pub const EAD_ZEROCONF_INFO_K_1_LABEL: u8 = 0x0;
-pub const EAD_ZEROCONF_INFO_IV_1_LABEL: u8 = 0x1;
-pub const EAD_ZEROCONF_ENC_STRUCTURE_LEN: usize = 2 + 8 + 3;
 
 pub type BytesSuites = [u8; SUITES_LEN];
 pub type BytesSupportedSuites = [u8; SUPPORTED_SUITES_LEN];
 pub const EDHOC_SUITES: BytesSuites = [0, 1, 2, 3, 4, 5, 6, 24, 25]; // all but private cipher suites
 pub const EDHOC_SUPPORTED_SUITES: BytesSupportedSuites = [0x2u8];
 
 pub type BytesEad2 = [u8; 0];
@@ -100,26 +98,172 @@
 pub type BytesMaxLabelBuffeer = [u8; MAX_KDF_LABEL_LEN];
 pub type BytesEncStructureLen = [u8; ENC_STRUCTURE_LEN];
 
 pub type BytesMac = [u8; MAC_LENGTH];
 pub type BytesEncodedVoucher = [u8; ENCODED_VOUCHER_LEN];
 pub type EADMessageBuffer = EdhocMessageBuffer; // TODO: make it of size MAX_EAD_SIZE_LEN
 
-#[repr(C)]
+/// Value of C_R or C_I, as chosen by ourself or the peer.
+///
+/// Semantically, this is a byte string of some length.
+///
+/// This currently only supports numeric values (see
+/// https://github.com/openwsn-berkeley/lakers/issues/258), but may support larger values in the
+/// future.
+#[derive(Debug, PartialEq, Eq, Copy, Clone)]
+// TODO: This should not be needed, there is nothing special about the value 0.
+#[derive(Default)]
+pub struct ConnId(u8);
+
+impl ConnId {
+    /// Construct a ConnId from the result of [`cbor_decoder::int_raw`], which is a
+    /// byte that represents a single positive or negative CBOR integer encoded in the 5 bits minor
+    /// type.
+    ///
+    /// Evolving from u8-only values, this could later interact with the decoder directly.
+    pub const fn from_int_raw(raw: u8) -> Self {
+        debug_assert!(raw >> 5 <= 1, "Major type is not an integer");
+        debug_assert!(raw & 0x1f < 24, "Value is not immediate");
+        Self(raw)
+    }
+
+    /// The bytes that form the identifier (an arbitrary byte string)
+    pub fn as_slice(&self) -> &[u8] {
+        core::slice::from_ref(&self.0)
+    }
+
+    /// The CBOR encoding of the identifier.
+    ///
+    /// For the 48 compact connection identifiers -24..=23, this is identical to the slice
+    /// representation:
+    ///
+    /// ```
+    /// # use lakers_shared::ConnId;
+    /// let c_i = ConnId::from_slice(&[0x04]).unwrap();
+    /// assert_eq!(c_i.as_cbor(), &[0x04]);
+    /// ```
+    ///
+    /// For other IDs, this contains an extra byte header (but those are currently unsupported):
+    ///
+    /// ```should_panic
+    /// # use lakers_shared::ConnId;
+    /// let c_i = ConnId::from_slice(&[0xff]).unwrap();
+    /// assert_eq!(c_i.as_cbor(), &[0x41, 0xff]);
+    /// ```
+    pub fn as_cbor(&self) -> &[u8] {
+        core::slice::from_ref(&self.0)
+    }
+
+    /// Try to construct a ConnId from a slice.
+    ///
+    /// This is the inverse of [Self::as_slice], and returns None if the identifier is too long
+    /// (or, if only the compact 48 values are supported, outside of that range).
+    ///
+    /// ```
+    /// # use lakers_shared::ConnId;
+    /// let c_i = &[0x04];
+    /// let c_i = ConnId::from_slice(c_i).unwrap();
+    /// assert!(c_i.as_slice() == &[0x04]);
+    ///
+    /// // So far, longer slices are unsupported
+    /// assert!(ConnId::from_slice(&[0x12, 0x34]).is_none());
+    /// ```
+    pub fn from_slice(input: &[u8]) -> Option<Self> {
+        if input.len() != 1 {
+            return None;
+        }
+        if input[0] >> 5 > 1 {
+            return None;
+        }
+        if input[0] & 0x1f >= 24 {
+            return None;
+        }
+        Some(Self(input[0]))
+    }
+}
+
 #[derive(PartialEq, Debug)]
+#[non_exhaustive]
 pub enum EDHOCError {
-    UnknownPeer = 1,
-    MacVerificationFailed = 2,
-    UnsupportedMethod = 3,
-    UnsupportedCipherSuite = 4,
-    ParsingError = 5,
-    EadLabelTooLongError = 6,
-    EadTooLongError = 7,
-    EADError = 8,
-    UnknownError = 9,
+    /// In an exchange, a credential was set as "expected", but the credential configured by the
+    /// peer did not match what was presented. This is more an application internal than an EDHOC
+    /// error: When the application sets the expected credential, that process should be informed
+    /// by the known details.
+    UnexpectedCredential,
+    MacVerificationFailed,
+    UnsupportedMethod,
+    UnsupportedCipherSuite,
+    ParsingError,
+    EadLabelTooLongError,
+    EadTooLongError,
+    /// An EAD was received that was either not known (and critical), or not understood, or
+    /// otherwise erroneous.
+    EADUnprocessable,
+    /// The credential or EADs could be processed (possibly by a third party), but the decision
+    /// based on that was to not to continue the EDHOC session.
+    ///
+    /// See also
+    /// <https://datatracker.ietf.org/doc/html/draft-ietf-lake-authz#name-edhoc-error-access-denied>
+    AccessDenied,
+}
+
+impl EDHOCError {
+    /// The ERR_CODE corresponding to the error
+    ///
+    /// Errors that refer to internal limitations (such as EadTooLongError) are treated the same
+    /// way as parsing errors, and return an unspecified error: Those are equivalent to limitations
+    /// of the parser, and a constrained system can not be expected to differentiate between "the
+    /// standard allows this but my number space is too small" and "this violates the standard".
+    ///
+    /// If an EDHOCError is returned through EDHOC, it will use this in its EDHOC error message.
+    ///
+    /// Note that this on its own is insufficient to create an error message: Additional ERR_INFO
+    /// is needed, which may or may not be available with the EDHOCError alone.
+    ///
+    /// TODO: Evolve the EDHOCError type such that all information needed is available.
+    pub fn err_code(&self) -> ErrCode {
+        use EDHOCError::*;
+        match self {
+            UnexpectedCredential => ErrCode::UNSPECIFIED,
+            MacVerificationFailed => ErrCode::UNSPECIFIED,
+            UnsupportedMethod => ErrCode::UNSPECIFIED,
+            UnsupportedCipherSuite => ErrCode::WRONG_SELECTED_CIPHER_SUITE,
+            ParsingError => ErrCode::UNSPECIFIED,
+            EadLabelTooLongError => ErrCode::UNSPECIFIED,
+            EadTooLongError => ErrCode::UNSPECIFIED,
+            EADUnprocessable => ErrCode::UNSPECIFIED,
+            AccessDenied => ErrCode::ACCESS_DENIED,
+        }
+    }
+}
+
+/// Representation of an EDHOC ERR_CODE
+#[repr(C)]
+pub struct ErrCode(pub NonZeroI16);
+
+impl ErrCode {
+    // The way these are initialized will be simplified once const_option is stable
+
+    pub const UNSPECIFIED: Self = ErrCode(match NonZeroI16::new(1) {
+        Some(v) => v,
+        _ => unreachable!(),
+    });
+    pub const WRONG_SELECTED_CIPHER_SUITE: Self = ErrCode(match NonZeroI16::new(2) {
+        Some(v) => v,
+        _ => unreachable!(),
+    });
+    pub const UNKNOWN_CREDENTIAL: Self = ErrCode(match NonZeroI16::new(3) {
+        Some(v) => v,
+        _ => unreachable!(),
+    });
+    // Code requested in https://datatracker.ietf.org/doc/html/draft-ietf-lake-authz
+    pub const ACCESS_DENIED: Self = ErrCode(match NonZeroI16::new(3333) {
+        Some(v) => v,
+        _ => unreachable!(),
+    });
 }
 
 #[derive(Debug)]
 #[repr(C)]
 pub struct InitiatorStart {
     pub suites_i: BytesSuites,
     pub suites_i_len: usize,
@@ -133,15 +277,15 @@
     pub g_y: BytesP256ElemLen, // ephemeral public key of myself
 }
 
 #[derive(Default, Debug)]
 pub struct ProcessingM1 {
     pub y: BytesP256ElemLen,
     pub g_y: BytesP256ElemLen,
-    pub c_i: u8,
+    pub c_i: ConnId,
     pub g_x: BytesP256ElemLen, // ephemeral public key of the initiator
     pub h_message_1: BytesHashLen,
 }
 
 #[derive(Default, Clone, Debug)]
 #[repr(C)]
 pub struct WaitM2 {
@@ -161,15 +305,15 @@
 pub struct ProcessingM2 {
     pub mac_2: BytesMac2,
     pub prk_2e: BytesHashLen,
     pub th_2: BytesHashLen,
     pub x: BytesP256ElemLen,
     pub g_y: BytesP256ElemLen,
     pub plaintext_2: EdhocMessageBuffer,
-    pub c_r: u8,
+    pub c_r: ConnId,
     pub ead_2: Option<EADItem>,
 }
 
 #[derive(Default, Debug)]
 #[repr(C)]
 pub struct ProcessedM2 {
     pub prk_3e2m: BytesHashLen,
@@ -463,28 +607,28 @@
         rcvd_message_1: &BufferMessage1,
     ) -> Result<
         (
             u8,
             BytesSuites,
             usize,
             BytesP256ElemLen,
-            u8,
+            ConnId,
             Option<EADItem>,
         ),
         EDHOCError,
     > {
         let mut decoder = CBORDecoder::new(rcvd_message_1.as_slice());
         let method = decoder.u8()?;
 
         if let Ok((suites_i, suites_i_len, mut decoder)) = parse_suites_i(decoder) {
             let mut g_x: BytesP256ElemLen = [0x00; P256_ELEM_LEN];
             g_x.copy_from_slice(decoder.bytes_sized(P256_ELEM_LEN)?);
 
             // consume c_i encoded as single-byte int (we still do not support bstr encoding)
-            let c_i = decoder.int_raw()?;
+            let c_i = ConnId::from_int_raw(decoder.int_raw()?);
 
             // if there is still more to parse, the rest will be the EAD_1
             if rcvd_message_1.len > decoder.position() {
                 // NOTE: since the current implementation only supports one EAD handler,
                 // we assume only one EAD item
                 let ead_res = parse_ead(decoder.remaining_buffer()?);
                 if let Ok(ead_1) = ead_res {
@@ -531,20 +675,20 @@
         } else {
             Err(EDHOCError::ParsingError)
         }
     }
 
     pub fn decode_plaintext_2(
         plaintext_2: &BufferCiphertext2,
-    ) -> Result<(u8, IdCred, BytesMac2, Option<EADItem>), EDHOCError> {
+    ) -> Result<(ConnId, IdCred, BytesMac2, Option<EADItem>), EDHOCError> {
         let mut mac_2: BytesMac2 = [0x00; MAC_LENGTH_2];
 
         let mut decoder = CBORDecoder::new(plaintext_2.as_slice());
 
-        let c_r = decoder.int_raw()?;
+        let c_r = ConnId::from_int_raw(decoder.int_raw()?);
 
         // NOTE: if len of bstr is 1, it is a compact kid and therefore should have been encoded as int
         let id_cred_r = if CBOR_MAJOR_BYTE_STRING == CBORDecoder::type_of(decoder.current()?)
             && CBORDecoder::info_of(decoder.current()?) > 1
         {
             IdCred::FullCredential(decoder.bytes()?)
         } else {
```

### Comparing `lakers_python-0.2.1/shared/src/python_bindings.rs` & `lakers_python-0.3.0/shared/src/python_bindings.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/crypto/lakers-crypto-psa/src/lib.rs` & `lakers_python-0.3.0/crypto/lakers-crypto-psa/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,21 @@
         let mut message: [u8; MAX_INFO_LEN + SHA256_DIGEST_LEN + 1] =
             [0; MAX_INFO_LEN + SHA256_DIGEST_LEN + 1];
         message[..info_len].copy_from_slice(&info[..info_len]);
         message[info_len] = 0x01;
         let mut t_i = self.hmac_sha256(&message[..info_len + 1], prk);
         output[..SHA256_DIGEST_LEN].copy_from_slice(&t_i);
 
-        for i in 2..n {
+        for i in 2..=n {
             message[..SHA256_DIGEST_LEN].copy_from_slice(&t_i);
             message[SHA256_DIGEST_LEN..SHA256_DIGEST_LEN + info_len]
                 .copy_from_slice(&info[..info_len]);
             message[SHA256_DIGEST_LEN + info_len] = i as u8;
             t_i = self.hmac_sha256(&message[..SHA256_DIGEST_LEN + info_len + 1], prk);
-            output[i * SHA256_DIGEST_LEN..(i + 1) * SHA256_DIGEST_LEN].copy_from_slice(&t_i);
+            output[(i - 1) * SHA256_DIGEST_LEN..i * SHA256_DIGEST_LEN].copy_from_slice(&t_i);
         }
 
         output[length..].fill(0x00);
 
         output
     }
```

### Comparing `lakers_python-0.2.1/lakers-python/Cargo.toml` & `lakers_python-0.3.0/lakers-python/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "lakers-python" # this will be the name of the package on pypi
 edition = "2021"
-version ="0.2.1"
+version ="0.3.0"
 repository.workspace = true
 license.workspace = true
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 pyo3 = { version = "0.20.2", features = ["extension-module"] }
 lakers = { package = "lakers", path = "../lib", default-features = false }
-lakers-ead = { path = "../ead/", features = [ "ead-authz" ] }
+lakers-ead-authz = { path = "../ead/lakers-ead-authz" }
 lakers-shared = { path = "../shared", features = ["python-bindings"] }
 lakers-crypto = { path = "../crypto", default-features = false, features = ["rustcrypto"] }
 
 [lib]
 name = "lakers" # this will be the name of the python package (as in `import lakers`), and it must match the module name in lib.rs
 crate-type = ["cdylib"]
```

### Comparing `lakers_python-0.2.1/lakers-python/README.md` & `lakers_python-0.3.0/lakers-python/README.md`

 * *Files identical despite different names*

### Comparing `lakers_python-0.2.1/lakers-python/src/ead_authz/authenticator.rs` & `lakers_python-0.3.0/lakers-python/src/ead_authz/authenticator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use lakers::*;
-use lakers_ead::*;
+use lakers_ead_authz::*;
 use pyo3::{
     prelude::*,
     types::{PyBytes, PyString},
 };
 
 #[pyclass(name = "AuthzAutenticator")]
 pub struct PyAuthzAutenticator {
```

### Comparing `lakers_python-0.2.1/lakers-python/src/ead_authz/device.rs` & `lakers_python-0.3.0/lakers-python/src/ead_authz/device.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use lakers::*;
 use lakers_crypto::default_crypto;
-use lakers_ead::*;
+use lakers_ead_authz::*;
 use pyo3::{exceptions::PyBaseException, prelude::*, types::PyBytes};
 
 #[pyclass(name = "AuthzDevice")]
 pub struct PyAuthzDevice {
     device: ZeroTouchDevice,
     device_wait: ZeroTouchDeviceWaitEAD2,
     device_done: ZeroTouchDeviceDone,
```

### Comparing `lakers_python-0.2.1/lakers-python/src/ead_authz/server.rs` & `lakers_python-0.3.0/lakers-python/src/ead_authz/server.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use lakers::*;
 use lakers_crypto::default_crypto;
-use lakers_ead::*;
+use lakers_ead_authz::*;
 use pyo3::{prelude::*, types::PyBytes};
 
 #[pyclass(name = "AuthzEnrollmentServer")]
 pub struct PyAuthzEnrollmentServer {
     server: ZeroTouchServer,
 }
```

### Comparing `lakers_python-0.2.1/lakers-python/src/initiator.rs` & `lakers_python-0.3.0/lakers-python/src/initiator.rs`

 * *Files 17% similar despite different names*

```diff
@@ -36,45 +36,49 @@
             completed: Completed::default(),
         }
     }
 
     fn prepare_message_1<'a>(
         &mut self,
         py: Python<'a>,
-        c_i: Option<u8>,
+        c_i: Option<Vec<u8>>,
         ead_1: Option<EADItem>,
     ) -> PyResult<&'a PyBytes> {
         let c_i = match c_i {
-            Some(c_i) => c_i,
+            Some(c_i) => ConnId::from_slice(c_i.as_slice()).ok_or(
+                pyo3::exceptions::PyValueError::new_err("Connection identifier out of range"),
+            )?,
             None => generate_connection_identifier_cbor(&mut default_crypto()),
         };
 
         match i_prepare_message_1(&self.start, &mut default_crypto(), c_i, &ead_1) {
             Ok((state, message_1)) => {
                 self.wait_m2 = state;
                 Ok(PyBytes::new(py, message_1.as_slice()))
             }
             Err(error) => Err(error.into()),
         }
     }
 
-    pub fn parse_message_2(
+    pub fn parse_message_2<'a>(
         &mut self,
+        py: Python<'a>,
         message_2: Vec<u8>,
-    ) -> PyResult<(u8, Vec<u8>, Option<EADItem>)> {
+    ) -> PyResult<(&'a PyBytes, &'a PyBytes, Option<EADItem>)> {
         let message_2 = EdhocMessageBuffer::new_from_slice(message_2.as_slice())?;
 
         match i_parse_message_2(&self.wait_m2, &mut default_crypto(), &message_2) {
             Ok((state, c_r, id_cred_r, ead_2)) => {
                 self.processing_m2 = state;
                 let id_cred_r = if id_cred_r.reference_only() {
-                    Vec::from([id_cred_r.kid])
+                    PyBytes::new(py, &[id_cred_r.kid])
                 } else {
-                    Vec::from(id_cred_r.value.as_slice())
+                    PyBytes::new(py, id_cred_r.value.as_slice())
                 };
+                let c_r = PyBytes::new(py, c_r.as_slice());
                 Ok((c_r, id_cred_r, ead_2))
             }
             Err(error) => Err(error.into()),
         }
     }
 
     pub fn verify_message_2(
@@ -107,25 +111,28 @@
     }
 
     pub fn prepare_message_3<'a>(
         &mut self,
         py: Python<'a>,
         cred_transfer: CredentialTransfer,
         ead_3: Option<EADItem>,
-    ) -> PyResult<(&'a PyBytes, [u8; SHA256_DIGEST_LEN])> {
+    ) -> PyResult<(&'a PyBytes, &'a PyBytes)> {
         match i_prepare_message_3(
             &mut self.processed_m2,
             &mut default_crypto(),
             self.cred_i.unwrap(),
             cred_transfer,
             &ead_3,
         ) {
             Ok((state, message_3, prk_out)) => {
                 self.completed = state;
-                Ok((PyBytes::new(py, message_3.as_slice()), prk_out))
+                Ok((
+                    PyBytes::new(py, message_3.as_slice()),
+                    PyBytes::new(py, prk_out.as_slice()),
+                ))
             }
             Err(error) => Err(error.into()),
         }
     }
 
     pub fn edhoc_exporter<'a>(
         &mut self,
```

### Comparing `lakers_python-0.2.1/lakers-python/src/lib.rs` & `lakers_python-0.3.0/lakers-python/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 /// This file implements the python bindings for the lakers library.
 /// Note that this module is not restricted by no_std.
 use lakers::*;
+// use lakers_ead_authz::consts::*;
 use lakers_crypto::{default_crypto, CryptoTrait};
 use pyo3::wrap_pyfunction;
 use pyo3::{prelude::*, types::PyBytes};
 
 mod ead_authz;
 mod initiator;
 mod responder;
@@ -70,9 +71,13 @@
     m.add_class::<lakers::CredentialTransfer>()?;
     m.add_class::<lakers::EADItem>()?;
     // ead-authz items
     m.add_class::<ead_authz::PyAuthzDevice>()?;
     m.add_class::<ead_authz::PyAuthzAutenticator>()?;
     m.add_class::<ead_authz::PyAuthzEnrollmentServer>()?;
     m.add_class::<ead_authz::PyAuthzServerUserAcl>()?;
+
+    let submodule = PyModule::new(_py, "consts")?;
+    submodule.add("EAD_AUTHZ_LABEL", lakers_ead_authz::consts::EAD_AUTHZ_LABEL)?;
+    m.add_submodule(submodule)?;
     Ok(())
 }
```

### Comparing `lakers_python-0.2.1/lakers-python/src/responder.rs` & `lakers_python-0.3.0/lakers-python/src/responder.rs`

 * *Files 15% similar despite different names*

```diff
@@ -29,31 +29,39 @@
             processing_m1: ProcessingM1::default(),
             wait_m3: WaitM3::default(),
             processing_m3: ProcessingM3::default(),
             completed: Completed::default(),
         }
     }
 
-    fn process_message_1(&mut self, message_1: Vec<u8>) -> PyResult<Option<EADItem>> {
+    fn process_message_1<'a>(
+        &mut self,
+        py: Python<'a>,
+        message_1: Vec<u8>,
+    ) -> PyResult<(&'a PyBytes, Option<EADItem>)> {
         let message_1 = EdhocMessageBuffer::new_from_slice(message_1.as_slice())?;
-        let (state, ead_1) = r_process_message_1(&self.start, &mut default_crypto(), &message_1)?;
+        let (state, c_i, ead_1) =
+            r_process_message_1(&self.start, &mut default_crypto(), &message_1)?;
         self.processing_m1 = state;
+        let c_i = PyBytes::new(py, c_i.as_slice());
 
-        Ok(ead_1)
+        Ok((c_i, ead_1))
     }
 
     fn prepare_message_2<'a>(
         &mut self,
         py: Python<'a>,
         cred_transfer: CredentialTransfer,
-        c_r: Option<u8>,
+        c_r: Option<Vec<u8>>,
         ead_2: Option<EADItem>,
     ) -> PyResult<&'a PyBytes> {
         let c_r = match c_r {
-            Some(c_r) => c_r,
+            Some(c_r) => ConnId::from_slice(c_r.as_slice()).ok_or(
+                pyo3::exceptions::PyValueError::new_err("Connection identifier out of range"),
+            )?,
             None => generate_connection_identifier_cbor(&mut default_crypto()),
         };
         let mut r = BytesP256ElemLen::default();
         r.copy_from_slice(self.r.as_slice());
 
         match r_prepare_message_2(
             &self.processing_m1,
@@ -68,38 +76,46 @@
                 self.wait_m3 = state;
                 Ok(PyBytes::new(py, message_2.as_slice()))
             }
             Err(error) => Err(error.into()),
         }
     }
 
-    pub fn parse_message_3(&mut self, message_3: Vec<u8>) -> PyResult<(Vec<u8>, Option<EADItem>)> {
+    pub fn parse_message_3<'a>(
+        &mut self,
+        py: Python<'a>,
+        message_3: Vec<u8>,
+    ) -> PyResult<(&'a PyBytes, Option<EADItem>)> {
         let message_3 = EdhocMessageBuffer::new_from_slice(message_3.as_slice())?;
         match r_parse_message_3(&mut self.wait_m3, &mut default_crypto(), &message_3) {
             Ok((state, id_cred_i, ead_3)) => {
                 self.processing_m3 = state;
                 let id_cred_i = if id_cred_i.reference_only() {
-                    Vec::from([id_cred_i.kid])
+                    PyBytes::new(py, &[id_cred_i.kid])
                 } else {
-                    Vec::from(id_cred_i.value.as_slice())
+                    PyBytes::new(py, id_cred_i.value.as_slice())
                 };
                 Ok((id_cred_i, ead_3))
             }
             Err(error) => Err(error.into()),
         }
     }
 
-    pub fn verify_message_3(&mut self, valid_cred_i: Vec<u8>) -> PyResult<[u8; SHA256_DIGEST_LEN]> {
+    pub fn verify_message_3<'a>(
+        &mut self,
+        py: Python<'a>,
+        valid_cred_i: Vec<u8>,
+    ) -> PyResult<&'a PyBytes> {
         let valid_cred_i = CredentialRPK::new(
             EdhocMessageBuffer::new_from_slice(&valid_cred_i.as_slice()).unwrap(),
         )?;
         match r_verify_message_3(&mut self.processing_m3, &mut default_crypto(), valid_cred_i) {
             Ok((state, prk_out)) => {
                 self.completed = state;
-                Ok(prk_out)
+                Ok(PyBytes::new(py, prk_out.as_slice()))
             }
             Err(error) => Err(error.into()),
         }
     }
 
     pub fn edhoc_exporter<'a>(
         &mut self,
```

### Comparing `lakers_python-0.2.1/lakers-python/test/test_ead_authz.py` & `lakers_python-0.3.0/lakers-python/test/test_ead_authz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import lakers
-import pytest
 
 # values from traces-zeroconf.ipynb
 ID_U = bytes.fromhex("a104412b")
 G_W = bytes.fromhex("FFA4F102134029B3B156890B88C9D9619501196574174DCB68A07DB0588E4D41")
 LOC_W = "coap://enrollment.server"
 W = bytes.fromhex("4E5E15AB35008C15B89E91F9F329164D4AACD53D9923672CE0019F9ACD98573F")
 KID_I = 0x2b
@@ -27,15 +26,15 @@
     ead_1 = lakers.EADItem(1, True, EAD_1_VALUE)
     loc_w, voucher_request = authenticator.process_ead_1(ead_1, MESSAGE_1_WITH_EAD)
     assert type(loc_w) == str
     voucher_response = enrollment_server.handle_voucher_request(voucher_request)
     assert type(voucher_response) == bytes
 
     ead_2 = authenticator.prepare_ead_2(voucher_response)
-    assert ead_2.label() == 1
+    assert ead_2.label() == lakers.consts.EAD_AUTHZ_LABEL
     assert ead_2.is_critical() == True
     assert ead_2.value() == EAD_2_VALUE
 
 def test_authenticator_and_server():
     VOUCHER_REQUEST_TV = bytes.fromhex("8158520382060258208af6f430ebe18d34184017a9a11bf511c8dff8f834730b96c1b7c8dbca2fc3b6370158287818636f61703a2f2f656e726f6c6c6d656e742e7365727665724dda9784962883c96ed01ff122c3")
     enrollment_server = lakers.AuthzServerUserAcl(W, CRED_V)
 
@@ -65,15 +64,15 @@
         initiator.compute_ephemeral_secret(device.get_g_w()),
         initiator.selected_cipher_suite(),
     )
     message_1 = initiator.prepare_message_1(c_i=None, ead_1=ead_1)
     device.set_h_message_1(initiator.get_h_message_1())
 
     # responder
-    ead_1 = responder.process_message_1(message_1)
+    _c_i, ead_1 = responder.process_message_1(message_1)
     loc_w, voucher_request = authenticator.process_ead_1(ead_1, message_1)
     voucher_response = enrollment_server.handle_voucher_request(voucher_request)
     ead_2 = authenticator.prepare_ead_2(voucher_response)
     message_2 = responder.prepare_message_2(lakers.CredentialTransfer.ByReference, None, ead_2)
     assert type(message_2) == bytes
 
     # initiator
```

### Comparing `lakers_python-0.2.1/lakers-python/test/test_lakers.py` & `lakers_python-0.3.0/lakers-python/test/test_lakers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import lakers
 import pytest
 
-# values from draft-ietf-lake-traces
+# values from RFC9529
 CRED_I = bytes.fromhex("A2027734322D35302D33312D46462D45462D33372D33322D333908A101A5010202412B2001215820AC75E9ECE3E50BFC8ED60399889522405C47BF16DF96660A41298CB4307F7EB62258206E5DE611388A4B8A8211334AC7D37ECB52A387D257E6DB3C2A93DF21FF3AFFC8")
 I = bytes.fromhex("fb13adeb6518cee5f88417660841142e830a81fe334380a953406a1305e8706b")
 R = bytes.fromhex("72cc4761dbd4c78f758931aa589d348d1ef874a7e303ede2f140dcf3e6aa4aac")
 CRED_R = bytes.fromhex("A2026008A101A5010202410A2001215820BBC34960526EA4D32E940CAD2A234148DDC21791A12AFBCBAC93622046DD44F02258204519E257236B2A0CE2023F0931F1F386CA7AFDA64FCDE0108C224C51EABF6072")
 CONTEXT = [0xa0, 0x11, 0x58, 0xfd, 0xb8, 0x20, 0x89, 0x0c, 0xd6, 0xbe, 0x16, 0x96, 0x02, 0xb8, 0xbc, 0xea]
 
 def test_gen_keys():
@@ -25,15 +25,15 @@
     initiator = lakers.EdhocInitiator()
     responder = lakers.EdhocResponder(R, CRED_R)
 
     # initiator
     message_1 = initiator.prepare_message_1(c_i=None, ead_1=None)
 
     # responder
-    ead_1 = responder.process_message_1(message_1)
+    _c_i, ead_1 = responder.process_message_1(message_1)
     assert ead_1 == None
     message_2 = responder.prepare_message_2(lakers.CredentialTransfer.ByReference, None, ead_1)
     assert type(message_2) == bytes
 
     # initiator
     c_r, id_cred_r, ead_2 = initiator.parse_message_2(message_2)
     assert ead_2 == None
@@ -53,15 +53,15 @@
     i_oscore_secret = initiator.edhoc_exporter(0, [], 16)
     i_oscore_salt = initiator.edhoc_exporter(1, [], 8)
     r_oscore_secret = responder.edhoc_exporter(0, [], 16)
     r_oscore_salt = responder.edhoc_exporter(1, [], 8)
     assert i_oscore_secret == r_oscore_secret
     assert i_oscore_salt == r_oscore_salt
 
-    # test key update with context from draft-ietf-lake-traces
+    # test key update with context from RFC9529
     i_prk_out_new = initiator.edhoc_key_update(CONTEXT)
     r_prk_out_new = responder.edhoc_key_update(CONTEXT)
     assert i_prk_out_new == r_prk_out_new
 
 def test_edhoc_error():
     responder = lakers.EdhocResponder(R, CRED_R)
     with pytest.raises(ValueError) as err:
```

### Comparing `lakers_python-0.2.1/Cargo.lock` & `lakers_python-0.3.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "abstract_integers"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e59b272bac6f8be86f13da69b4bab6fa79973ac6a745a8d4aece4f08aa00df56"
-dependencies = [
- "num",
- "num-bigint",
-]
-
-[[package]]
 name = "addr2line"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
 dependencies = [
  "gimli",
 ]
@@ -35,17 +25,17 @@
 dependencies = [
  "crypto-common",
  "generic-array 0.14.7",
 ]
 
 [[package]]
 name = "aes"
-version = "0.8.4"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b169f7a6d4742236a0a00c541b845991d0ac43e546831af1249753ab4c3aa3a0"
+checksum = "ac1f845298e95f983ff1944b728ae08b8cebab80d684f0a832ed0fc74dfa27e2"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
@@ -54,20 +44,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "alloc-traits"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b2d54853319fd101b8dd81de382bcbf3e03410a64d8928bbee85a3e7dcde483"
-
-[[package]]
 name = "ansi_term"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
@@ -131,20 +115,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5deb64efa5bd81e31fcd1938615a6d98c82eafcbcd787162b6f63b91d6bac5b3"
 dependencies = [
  "rustc_version 0.2.3",
 ]
 
 [[package]]
-name = "bare-metal"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8fe8f5a8a398345e52358e18ff07cc17a568fbca5c6f73873d3a62056309603"
-
-[[package]]
 name = "base16ct"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "bindgen"
@@ -167,32 +145,32 @@
  "rustc-hash",
  "shlex",
  "which",
 ]
 
 [[package]]
 name = "bindgen"
-version = "0.69.4"
+version = "0.69.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
+checksum = "a4c69fae65a523209d34240b60abe0c42d33d1045d445c0839d8a4894a736e2d"
 dependencies = [
  "bitflags 2.4.2",
  "cexpr",
  "clang-sys",
- "itertools",
  "lazy_static",
  "lazycell",
  "log",
+ "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.52",
+ "syn 2.0.48",
  "which",
 ]
 
 [[package]]
 name = "bitfield"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -216,20 +194,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array 0.14.7",
 ]
 
 [[package]]
-name = "build_const"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4ae4235e6dac0694637c763029ecea1a2ec9e4e06ec2729bd21ba4d9c863eb7"
-
-[[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
@@ -254,45 +226,19 @@
  "syn 1.0.109",
  "tempfile",
  "toml",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.89"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0ba8f7aaa012f30d5b2861462f6708eccd49c3c39863fe083a308035f63d723"
-
-[[package]]
-name = "cc2538-hal"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "341676d9ffe969cf2706c4b555dfaae6eb3810a14a90ed6577114920de89c92c"
-dependencies = [
- "cc2538-pac",
- "circular-queue",
- "cortex-m",
- "cortex-m-rt",
- "embedded-hal 1.0.0-alpha.5",
- "nb 1.1.0",
- "panic-rtt-target",
- "paste",
- "rtt-target 0.4.0",
-]
-
-[[package]]
-name = "cc2538-pac"
-version = "0.4.1"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58344c577d15817cecc2ede079f73ae9e9d5bf8b59c79dba7151e22ca24aba62"
+checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
 dependencies = [
- "bare-metal 1.0.0",
- "cortex-m",
- "cortex-m-rt",
- "vcell",
+ "libc",
 ]
 
 [[package]]
 name = "ccm"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae3c82e4355234767756212c570e29833699ab63e6ffd161887314cc5b43847"
@@ -316,38 +262,29 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.2"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
-name = "circular-queue"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d34327ead1c743a10db339de35fb58957564b99d248a67985c55638b22c59b5"
-dependencies = [
- "version_check",
-]
-
-[[package]]
 name = "clang-sys"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
 dependencies = [
  "glob",
  "libc",
@@ -377,15 +314,15 @@
 dependencies = [
  "atty",
  "bitflags 1.3.2",
  "clap_lex",
  "indexmap",
  "strsim 0.10.0",
  "termcolor",
- "textwrap 0.16.1",
+ "textwrap 0.16.0",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
@@ -406,22 +343,23 @@
 name = "coap"
 version = "0.1.0"
 dependencies = [
  "coap 0.13.0",
  "coap-handler",
  "coap-handler-implementations",
  "coap-lite",
- "coap-message 0.2.3",
+ "coap-message",
+ "coap-message-utils",
  "coap-numbers",
  "embedded-nal",
  "embedded-nal-minimal-coapserver",
  "hexlit",
  "lakers",
  "lakers-crypto",
- "lakers-ead",
+ "lakers-ead-authz",
  "std-embedded-nal",
 ]
 
 [[package]]
 name = "coap"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -441,79 +379,83 @@
  "tokio-stream",
  "tokio-util",
  "url",
 ]
 
 [[package]]
 name = "coap-handler"
-version = "0.1.6"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a2c21db09a4ce20cdf7153ed88b678f728aa8698109203e7f3087b12628e19"
+checksum = "8600ae8e54c9be6e0c5273fad0503e12f827742e4e3fea5a521412478d603b72"
 dependencies = [
- "byteorder",
- "coap-message 0.2.3",
+ "coap-message",
  "coap-numbers",
- "crc 1.8.1",
- "serde",
- "serde_cbor",
- "windowed-infinity",
 ]
 
 [[package]]
 name = "coap-handler-implementations"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f96e53455f4b1eadadadf53bef28d799dc295414bb2c8b8f86b3d45cc71f154"
+checksum = "f2735f53da500caae442466ba2126d62458e86116ec1e273919880410f7e187b"
 dependencies = [
  "ciborium-io",
  "coap-handler",
- "coap-message 0.2.3",
+ "coap-message",
+ "coap-message-utils",
  "coap-numbers",
- "crc 3.0.1",
+ "crc",
+ "document-features",
  "embedded-io",
  "minicbor",
  "serde",
  "serde_cbor",
  "windowed-infinity",
 ]
 
 [[package]]
 name = "coap-lite"
-version = "0.11.5"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d72f4fbcb650652c4b7d980390cf8af49a738422ac66718bd516ec3430b83a6"
+checksum = "25ca11cbc756cf12eb24824285dbe36d97e4cfea404aaa1240477f3ae091f779"
 dependencies = [
- "coap-message 0.2.3",
- "coap-message 0.3.1",
  "lru_time_cache",
 ]
 
 [[package]]
 name = "coap-message"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cc888e15f6be910b58fda4f056f673f58fb9348ea45da014283a14e6d2b58ec"
-
-[[package]]
-name = "coap-message"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae18782d02e6afdfcfaf48eb7ec591b0cae57b67b637441a490752d4a57db02f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "coap-message-implementations"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34293ae8447d52635184f556489bad7fa564d94cde3d00b170e2727964bc3645"
+dependencies = [
+ "coap-message",
+ "coap-message-utils",
+ "coap-numbers",
+ "heapless 0.5.6",
+]
+
+[[package]]
 name = "coap-message-utils"
-version = "0.2.2"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83241a72558f8b529ed7f29693a1621f66d9feced1a040af9db68f374e1981"
+checksum = "2ebb49f08ced17ea3a47a9206d99186849665854cea1fd064509008ed0cdfc4b"
 dependencies = [
- "coap-message 0.2.3",
+ "coap-message",
+ "coap-numbers",
+ "document-features",
  "heapless 0.5.6",
+ "minicbor",
 ]
 
 [[package]]
 name = "coap-numbers"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e766be4563107bc11c281c017ab922c3f3079345c9aa0fe747b4f9abc13411ac"
@@ -526,18 +468,18 @@
 
 [[package]]
 name = "cortex-m"
 version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ec610d8f49840a5b376c69663b6369e71f4b34484b9b2eb29fb918d92516cb9"
 dependencies = [
- "bare-metal 0.2.5",
+ "bare-metal",
  "bitfield",
  "critical-section",
- "embedded-hal 0.2.7",
+ "embedded-hal",
  "volatile-register",
 ]
 
 [[package]]
 name = "cortex-m-rt"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -573,23 +515,14 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc"
-version = "1.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d663548de7f5cca343f1e0a48d14dcfb0e9eb4e079ec58883b7251539fa10aeb"
-dependencies = [
- "build_const",
-]
-
-[[package]]
-name = "crc"
 version = "3.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86ec7a15cbe22e59248fc7eadb1907dab5ba09372595da4d73dd805ed4417dfe"
 dependencies = [
  "crc-catalog",
 ]
 
@@ -654,34 +587,27 @@
 dependencies = [
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
-name = "edhoc-cc2538"
-version = "0.1.0"
+name = "document-features"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
 dependencies = [
- "cc2538-hal",
- "cc2538-pac",
- "cortex-m",
- "cortex-m-rt",
- "embedded-alloc",
- "hexlit",
- "lakers",
- "lakers-crypto",
- "panic-rtt-target",
- "rtt-target 0.3.1",
+ "litrs",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "elliptic-curve"
 version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
@@ -715,23 +641,14 @@
 checksum = "35949884794ad573cf46071e41c9b60efb0cb311e3ca01f7af807af1debc66ff"
 dependencies = [
  "nb 0.1.3",
  "void",
 ]
 
 [[package]]
-name = "embedded-hal"
-version = "1.0.0-alpha.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a554c04648665230499563ccdfd1fcd719ef2d5a0af54bdc81c5d877fb556db4"
-dependencies = [
- "nb 1.1.0",
-]
-
-[[package]]
 name = "embedded-io"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef1a6892d9eef45c8fa6b9e0086428a2cca8491aca8f787c534a3d6d0bcb3ced"
 
 [[package]]
 name = "embedded-nal"
@@ -742,21 +659,21 @@
  "heapless 0.7.17",
  "nb 1.1.0",
  "no-std-net",
 ]
 
 [[package]]
 name = "embedded-nal-minimal-coapserver"
-version = "0.3.1"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38c69bec57fe2be900d6a95696e933a25b2bb54b0be5f4df20822fb415e4fdbf"
+checksum = "b6e7e827cbc4f6bf46b9973946396e7e3dae3e0d34aa8e560924b7d62dbcaf55"
 dependencies = [
  "coap-handler",
- "coap-message 0.2.3",
- "coap-message-utils",
+ "coap-message",
+ "coap-message-implementations",
  "coap-numbers",
  "embedded-nal",
  "heapless 0.5.6",
  "num-derive",
  "num-traits",
 ]
 
@@ -860,15 +777,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -957,29 +874,18 @@
 dependencies = [
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
-name = "hacspec-lib"
-version = "0.1.0-beta.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c419ad52a9b12ce9ad821d5f9b8e59cff4f241aacf096e7559c8fa4600148343"
-dependencies = [
- "abstract_integers",
- "num",
- "secret_integers",
-]
-
-[[package]]
 name = "half"
-version = "1.8.3"
+version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b43ede17f21864e81be2fa654110bf1e793774238d86ef8555c37e6519c0403"
+checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
 name = "hash32"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4041af86e63ac4298ce40e5cca669066e75b6f1aa3390fe2561ffa5e1d9f4cc"
 dependencies = [
@@ -1039,17 +945,17 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.9"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
+checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
 
 [[package]]
 name = "hexlit"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b6e75c860d4216ac53f9ac88b25c99eaedba075b3a7b2ed31f2adc51a74fffd"
 
@@ -1118,84 +1024,61 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
  "generic-array 0.14.7",
 ]
 
 [[package]]
-name = "itertools"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
-dependencies = [
- "either",
-]
-
-[[package]]
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "lakers"
 version = "0.5.1"
 dependencies = [
  "hexlit",
  "lakers-crypto",
- "lakers-ead",
+ "lakers-ead-authz",
  "lakers-shared",
 ]
 
 [[package]]
 name = "lakers-c"
 version = "0.5.1"
 dependencies = [
  "cbindgen",
  "critical-section",
  "embedded-alloc",
  "hexlit",
  "lakers",
  "lakers-crypto",
- "lakers-ead",
+ "lakers-ead-authz",
  "panic-semihosting",
 ]
 
 [[package]]
 name = "lakers-crypto"
 version = "0.5.1"
 dependencies = [
- "lakers-crypto-cc2538",
+ "hexlit",
  "lakers-crypto-cryptocell310",
  "lakers-crypto-psa",
  "lakers-crypto-rustcrypto",
  "lakers-shared",
  "rand_core",
-]
-
-[[package]]
-name = "lakers-crypto-cc2538"
-version = "0.5.1"
-dependencies = [
- "cc2538-hal",
- "cc2538-pac",
- "cortex-m",
- "cortex-m-rt",
- "cortex-m-semihosting",
- "hacspec-lib",
- "lakers-shared",
- "panic-semihosting",
- "static-alloc",
+ "rstest",
 ]
 
 [[package]]
 name = "lakers-crypto-cryptocell310"
 version = "0.5.1"
 dependencies = [
- "bindgen 0.69.4",
+ "bindgen 0.69.2",
  "lakers-shared",
 ]
 
 [[package]]
 name = "lakers-crypto-psa"
 version = "0.5.1"
 dependencies = [
@@ -1214,22 +1097,14 @@
  "lakers-shared",
  "p256",
  "rand_core",
  "sha2",
 ]
 
 [[package]]
-name = "lakers-ead"
-version = "0.5.1"
-dependencies = [
- "lakers-ead-authz",
- "lakers-shared",
-]
-
-[[package]]
 name = "lakers-ead-authz"
 version = "0.5.1"
 dependencies = [
  "hexlit",
  "lakers-crypto",
  "lakers-shared",
 ]
@@ -1241,26 +1116,26 @@
  "cortex-m",
  "cortex-m-rt",
  "cortex-m-semihosting",
  "embedded-alloc",
  "hexlit",
  "lakers",
  "lakers-crypto",
- "lakers-ead",
+ "lakers-ead-authz",
  "panic-semihosting",
- "rtt-target 0.3.1",
+ "rtt-target",
 ]
 
 [[package]]
 name = "lakers-python"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "lakers",
  "lakers-crypto",
- "lakers-ead",
+ "lakers-ead-authz",
  "lakers-shared",
  "pyo3",
 ]
 
 [[package]]
 name = "lakers-shared"
 version = "0.5.1"
@@ -1279,26 +1154,26 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
 
 [[package]]
 name = "libloading"
-version = "0.8.2"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2caa5afb8bf9f3a2652760ce7d4f62d21c4d5a423e68466fca30df82f2330164"
+checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "linked_list_allocator"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9afa463f5405ee81cdb9cc2baf37e08ec7e4c8209442b5d72c04cfb2cd6e6286"
@@ -1306,28 +1181,34 @@
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
+name = "litrs"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4ce301924b7887e9d637144fdade93f9dfff9b60981d4ac161db09720d39aa5"
+
+[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.21"
+version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
+checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
 name = "lru_time_cache"
 version = "0.11.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9106e1d747ffd48e6be5bb2d97fa706ed25b144fbee4d5c02eae110cd8d6badd"
 
@@ -1356,17 +1237,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.8"
@@ -1407,104 +1288,40 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
-name = "num"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
-dependencies = [
- "num-complex",
- "num-integer",
- "num-iter",
- "num-rational",
- "num-traits",
-]
-
-[[package]]
-name = "num-bigint"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
-name = "num-complex"
-version = "0.4.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
 name = "num-derive"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.46"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-iter"
-version = "0.1.44"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
-name = "num-rational"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.3.9",
+ "hermit-abi 0.3.3",
  "libc",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1532,24 +1349,14 @@
 checksum = "c9863ad85fa8f4460f9c48cb909d38a0d689dba1f6f6988a5e3e0d31071bcd4b"
 dependencies = [
  "elliptic-curve",
  "primeorder",
 ]
 
 [[package]]
-name = "panic-rtt-target"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d6ab67bc881453e4c90f958c657c1303670ea87bc1a16e87fd71a40f656dce9"
-dependencies = [
- "cortex-m",
- "rtt-target 0.3.1",
-]
-
-[[package]]
 name = "panic-semihosting"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee8a3e1233d9073d76a870223512ce4eeea43c067a94a445c13bd6d792d7b1ab"
 dependencies = [
  "cortex-m",
  "cortex-m-semihosting",
@@ -1575,20 +1382,14 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "paste"
-version = "1.0.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
-
-[[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "percent-encoding"
@@ -1605,43 +1406,37 @@
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
-name = "portable-atomic"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
-
-[[package]]
 name = "prettyplease"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
 dependencies = [
  "proc-macro2",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "primeorder"
 version = "0.13.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "353e1ca18966c16d9deb1c69278edbc5f194139612772bd9537af60ac231e1e6"
 dependencies = [
  "elliptic-curve",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.76"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psa-crypto"
 version = "0.9.2"
@@ -1662,73 +1457,71 @@
  "cc",
  "cmake",
  "walkdir",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
- "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
 dependencies = [
  "heck",
  "proc-macro2",
- "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -1752,58 +1545,61 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.6"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
+checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
-name = "rtt-target"
-version = "0.3.1"
+name = "rstest"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065d6058bb1204f51a562a67209e1817cf714759d5cf845aa45c75fa7b0b9d9b"
+checksum = "2288c66aeafe3b2ed227c981f364f9968fa952ef0b30e84ada4486e7ee24d00a"
 dependencies = [
- "cortex-m",
- "ufmt-write",
+ "cfg-if",
+ "proc-macro2",
+ "quote",
+ "rustc_version 0.4.0",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "rtt-target"
-version = "0.4.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3afa12c77ba1b9bf560e4039a9b9a08bb9cde0e9e6923955eeb917dd8d5cf303"
+checksum = "065d6058bb1204f51a562a67209e1817cf714759d5cf845aa45c75fa7b0b9d9b"
 dependencies = [
- "critical-section",
+ "cortex-m",
  "ufmt-write",
 ]
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1826,35 +1622,35 @@
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
- "semver 1.0.22",
+ "semver 1.0.21",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "322394588aaf33c24007e8bb3238ee3e4c5c09c084ab32bc73890b99ff326bca"
 dependencies = [
  "bitflags 2.4.2",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1877,45 +1673,39 @@
  "der",
  "generic-array 0.14.7",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
-name = "secret_integers"
-version = "0.1.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6267ec5e8c6409b7616e40fbcda431c016271d245e93aa850ffda8f5e1bfa36f"
-
-[[package]]
 name = "semver"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d7eb9ef2c18661902cc47e535f9bc51b78acd254da71d375c2f6720d9a40403"
 dependencies = [
  "semver-parser",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "b97ed7a9823b74f99c7742f5336af7be5ecd3eeafcb1507d1fa93347b1d589b0"
 
 [[package]]
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.195"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -1924,28 +1714,28 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.195"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.111"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1957,17 +1747,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "shlex"
-version = "1.3.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
+checksum = "a7cee0529a6d40f580e7a5e6c495c8fbfe21b7b52795ed4bb5e62cdf92bc6380"
 
 [[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
@@ -1981,26 +1771,26 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "2593d31f82ead8df961d8bd23a64c2ccf2eb5dd34b0a34bfb4dd54011c72009e"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
 dependencies = [
  "libc",
- "windows-sys 0.52.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
@@ -2011,23 +1801,14 @@
 [[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
-name = "static-alloc"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b2975e035ce16539eecee08d7c6e5626ca26f299c6e90af343b302c6dd2e61e"
-dependencies = [
- "alloc-traits",
-]
-
-[[package]]
 name = "std-embedded-nal"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f015e1ff920d670d8d11c7560a9a91bb6dde2d7bb530ed556aadc58878a37809"
 dependencies = [
  "embedded-nal",
 ]
@@ -2059,37 +1840,38 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.48"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.14"
+version = "0.12.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
+checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
 
 [[package]]
 name = "tempfile"
-version = "3.10.1"
+version = "3.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
+checksum = "01ce4141aa927a6d1bd34a041795abd0db1cccba5d5f24b009f694bdf3a1f3fa"
 dependencies = [
  "cfg-if",
  "fastrand",
+ "redox_syscall",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
@@ -2106,17 +1888,17 @@
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "textwrap"
-version = "0.16.1"
+version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
+checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
@@ -2152,15 +1934,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
@@ -2203,29 +1985,29 @@
 name = "ufmt-write"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e87a2ed6b42ec5e28cc3b94c09982969e9227600b2e3dcbc1db927a84c06bd69"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.15"
+version = "0.3.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
+checksum = "6f2528f27a9eb2b21e69c95319b30bd0efd85d09c379741b0f78ea1d86be2416"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.23"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
 version = "0.1.11"
@@ -2280,17 +2062,17 @@
 checksum = "de437e2a6208b014ab52972a27e59b33fa2920d3e00fe05026167a1c509d19cc"
 dependencies = [
  "vcell",
 ]
 
 [[package]]
 name = "walkdir"
-version = "2.5.0"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
+checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
@@ -2344,15 +2126,15 @@
 [[package]]
 name = "windowed-infinity"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c9487d1d565a9db59e1fd0b3c2d3f0c277bc375d348a6c46ff2b322917fbc035"
 dependencies = [
  "ciborium-io",
- "crc 3.0.1",
+ "crc",
  "digest",
  "embedded-io",
  "minicbor",
  "serde",
  "serde_cbor",
 ]
 
@@ -2367,15 +2149,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2387,110 +2169,110 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.0",
+ "windows_aarch64_msvc 0.52.0",
+ "windows_i686_gnu 0.52.0",
+ "windows_i686_msvc 0.52.0",
+ "windows_x86_64_gnu 0.52.0",
+ "windows_x86_64_gnullvm 0.52.0",
+ "windows_x86_64_msvc 0.52.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 dependencies = [
@@ -2501,9 +2283,9 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.48",
 ]
```

### Comparing `lakers_python-0.2.1/Cargo.toml` & `lakers_python-0.3.0/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 members = ["lakers-python"]
 
 # reduced "default-members", should include only packages that can be built and
 # tested on the host architecture
 default-members = [
   "lib",
-  "ead",
   "crypto",
   "crypto/lakers-crypto-rustcrypto",
   "examples/coap",
 ]
 
 # according to https://doc.rust-lang.org/edition-guide/rust-2021/default-cargo-resolver.html,
 # this needs to be explicitly set if using virtual manifests (like this).
@@ -20,32 +19,25 @@
 resolver = "2"
 
 [workspace.package]
 version = "0.5.1"
 repository = "https://github.com/openwsn-berkeley/lakers/"
 license = "BSD-3-Clause"
 readme = "shared/README.md"
+keywords = ["iot", "security", "protocol", "crypto", "edhoc"]
+categories = [ "no-std::no-alloc", "network-programming", "embedded" ]
 
 [workspace.dependencies]
 
 lakers-shared = { package = "lakers-shared", path = "shared/", version = "^0.5.1" }
 
-lakers-ead = { package = "lakers-ead", path = "ead/", version = "^0.5.1", default-features = false }
 lakers-ead-authz = { package = "lakers-ead-authz", path = "ead/lakers-ead-authz/", version = "^0.5.1" }
 
 lakers-crypto = { path = "crypto/" }
-lakers-crypto-cc2538 = { path = "crypto/lakers-crypto-cc2538/" }
 lakers-crypto-cryptocell310 = { path = "crypto/lakers-crypto-cryptocell310-sys/" }
-# lakers-crypto-hacspec = { path = "crypto/lakers-crypto-hacspec/" }
 lakers-crypto-psa = { path = "crypto/lakers-crypto-psa/" }
 lakers-crypto-rustcrypto = { package = "lakers-crypto-rustcrypto", path = "crypto/lakers-crypto-rustcrypto/", version = "^0.5.1" }
 
 lakers = { package = "lakers", path = "lib/", version = "^0.5.1", default-features = false }
 
 [patch.crates-io]
-# hacspec-lib = { git = "https://github.com/malishav/hacspec", branch = "aesccm" }
-# hacspec-p256 = { git = "https://github.com/malishav/hacspec", branch = "aesccm" }
-# hacspec-hkdf = { git = "https://github.com/malishav/hacspec", branch = "aesccm" }
-# hacspec-sha256 = { git = "https://github.com/malishav/hacspec", branch = "aesccm" }
-# hacspec-aes = { git = "https://github.com/malishav/hacspec", branch = "aesccm" }
-# hacspec-aes-ccm = { git = "https://github.com/malishav/hacspec", branch = "aesccm" }
 psa-crypto = { git = "https://github.com/malishav/rust-psa-crypto", branch = "baremetal" }
```

### Comparing `lakers_python-0.2.1/PKG-INFO` & `lakers_python-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: lakers-python
-Version: 0.2.1
+Version: 0.3.0
 License: BSD-3-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/openwsn-berkeley/lakers/
 
 # Lakers Python
 Python wrapper for the [`lakers` crate](https://github.com/openwsn-berkeley/lakers).
```


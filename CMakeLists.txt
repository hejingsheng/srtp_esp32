idf_component_register(SRCS "srtp/srtp.c"
							"srtp/ekt.c"
							"crypto/cipher/aes_icm.c"
							"crypto/cipher/aes.c"
							"crypto/cipher/cipher.c"
							"crypto/cipher/null_cipher.c"
							"crypto/hash/auth.c"
							"crypto/hash/hmac.c"
							"crypto/hash/null_auth.c"
							"crypto/hash/sha1.c"
							"crypto/kernel/alloc.c"
							"crypto/kernel/crypto_kernel.c"
							"crypto/kernel/err.c"
							"crypto/kernel/key.c"
							"crypto/math/datatypes.c"
							"crypto/math/stat.c"
							"crypto/replay/rdb.c"
							"crypto/replay/rdbx.c"
							"crypto/replay/ut_sim.c"
                    INCLUDE_DIRS "include" "crypto/include")
                   
 target_compile_options(${COMPONENT_LIB} PRIVATE -DHAVE_CONFIG_H)


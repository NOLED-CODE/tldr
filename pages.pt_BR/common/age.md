age

>Uma ferramenta simples, moderna e segura de criptografia de arquivos. Veja também: age-keygen para gerar pares de chaves. Mais informações: https://github.com/FiloSottile/age.
>
Gerar um arquivo criptografado que pode ser descriptografado com uma senha:
>
`age --passphrase --output {{caminho/para/arquivo_criptografado}} {{caminho/para/arquivo_nao_criptografado}}`

Criptografar um arquivo com uma ou mais chaves públicas inseridas como literais (repita a flag --recipient para especificar várias chaves públicas):

`age --recipient {{chave_publica}} --output {{caminho/para/arquivo_criptografado}} {{caminho/para/arquivo_nao_criptografado}}`

Criptografar um arquivo para um ou mais destinatários cujas chaves públicas estão especificadas em um arquivo (uma por linha):

`age --recipients-file {{caminho/para/arquivo_de_destinatarios}} --output {{caminho/para/arquivo_criptografado}} {{caminho/para/arquivo_nao_criptografado}}`

Descriptografar um arquivo com uma senha:

`age --decrypt --output {{caminho/para/arquivo_descriptografado}} {{caminho/para/arquivo_criptografado}}`

Descriptografar um arquivo com um arquivo de chave privada:

`age --decrypt --identity {{caminho/para/arquivo_de_chave_privada}} --output {{caminho/para/arquivo_descriptografado}} {{caminho/para/arquivo_criptografado}}`

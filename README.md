after buying ssl, provider give you three file:
certificate.crt
bundle.crt
private.key

for caddy you should genrate two file:
chain.pem
key.pm

run this command for generate chain.pm and key.pm:
cat ./new/cert.crt ./new/bundle.crt > ./ssl/chain.pem && cat ./new/priv.key > ./ssl/key.pem 

now copy key.pem and chain.pem to the caddy ssl folder
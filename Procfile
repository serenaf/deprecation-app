release: if [ -z "$FASTLY_PURGE_KEY" ]; then echo "Skipping Fastly purge because FASTLY_PURGE_KEY is not set"; else curl --silent --show-error --fail -XPOST -H "Fastly-Key:$FASTLY_PURGE_KEY" https://api.fastly.com/service/$FASTLY_SERVICE_ID/purge_all; fi

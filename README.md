# online
yarn config set yarn-offline-mirror ./npm-packages-offline-cache

yarn config set yarn-offline-mirror-pruning true
# tar
tar -czf 1 /usr/local/share/npm-packages-offline-cache
# untar
tar -xzf 1
# offline
yarn config set yarn-offline-mirror ./npm-packages-offline-cache

yarn config set yarn-offline-mirror-pruning true

yarn cache clean

yarn install -offline

yarn install

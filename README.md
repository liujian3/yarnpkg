# online
yarn config set yarn-offline-mirror ./npm-packages-offline-cache

yarn config set yarn-offline-mirror-pruning true
# offline
yarn config set yarn-offline-mirror ./npm-packages-offline-cache

yarn config set yarn-offline-mirror-pruning true

yarn cache clean

yarn install -offline

yarn install

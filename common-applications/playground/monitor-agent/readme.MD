### prometheus agent deploy
1. update global.external_labels.cluster and scrape_configs.job_name in configmap.yaml
2. update env AGENT_CONFIG in prometheus-agent.yaml
3. kustomize build . | kubectl apply -f -
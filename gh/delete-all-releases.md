```gh release list --repo ${REPO_NAME} | awk '{print $1}' | xargs -n 1 gh release delete --repo ${REPO_NAME}```

`xargs -n 1` takes one input argument for tools, so no need for loops


```bash
ovhai notebook run one-for-all jupyterlab \
--name colab-to-ovh \
--framework-version v98-ovh.beta.1 \
--volume myprivatecontainer@GRA/nb-data:/workspace/data:RO:cache \
--volume ai-notebook@GRA/:/workspace/saved_model:RWD \
--volume https://github.com/Victor2103/python_example_chatbot.git:/workspace/public-repo-git:RO \
--cpu 10
```
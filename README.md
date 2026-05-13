# NLP 作业汇总

Streamlit 单文件应用，整合 `nlp1.py` 到 `nlp9.py` 的九次作业界面。

## 本地运行

```bash
pip install -r requirements.txt
streamlit run nlp_all_homeworks.py
```

## 在线部署

GitHub 只负责托管代码；交互式 Streamlit 应用需要部署到 Streamlit Community Cloud。

1. 将本目录推送到 GitHub 仓库。
2. 打开 Streamlit Community Cloud。
3. New app，选择该 GitHub 仓库。
4. Main file path 填写：

```text
nlp_all_homeworks.py
```

5. Advanced settings 里将 Python version 选择为 `3.11`。
6. Deploy。

注意：如果日志里显示 `Using Python 3.14.x environment`，部分 NLP 依赖（例如 `gensim`、`spacy`）可能没有可用 wheel，会在安装阶段失败。已部署应用无法直接切换 Python 版本；需要删除 app 后用同一个仓库和子域名重新部署，并在 Advanced settings 里选择 Python 3.11。

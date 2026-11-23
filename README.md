# Insight AI no Streamlit

1. Extraia o ZIP e envie seu conteúdo à raiz de um repositório GitHub. Inclua a pasta `exemplos`.
2. Acesse https://share.streamlit.io/, clique em **Create app** e selecione seu repositório e branch.
3. Em **Main file path**, coloque `app.py`.
4. Para ativar a aba Gemini, coloque sua chave em **Advanced settings → Secrets**:

   ```toml
   GEMINI_API_KEY = "SUA_CHAVE"
   ```

5. Clique em **Deploy**. O dashboard e os exemplos funcionam sem chave.

Para executar localmente, instale com `python -m pip install -r requirements.txt` e rode
`python -m streamlit run app.py`. Se quiser usar o Gemini, defina a variável de ambiente
`GEMINI_API_KEY` ou crie `.streamlit/secrets.toml` com o conteúdo acima. Mantenha a chave fora do GitHub.

Esta edição usa a interface nativa do Streamlit. A aba Gemini trabalha com estatísticas agregadas.

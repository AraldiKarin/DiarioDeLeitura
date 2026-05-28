# 📚 Diário de Leitura

Um aplicativo web simples e delicado para registrar suas fichas de leitura — os livros que você leu, com capa, avaliação, datas e até o personagem favorito. Visual minimalista em tons pastéis, com sincronização na nuvem para acessar de qualquer dispositivo.

**🔗 Acesse o site:** https://araldikarin.github.io/diario-de-leitura/

---

## ✨ Funcionalidades

- **Fichas completas** para cada livro:
  - Título e autor
  - Coleção (opcional) — relacione a uma coleção existente ou crie uma nova
  - Data de início e data de fim da leitura (com cálculo automático de quantos dias durou)
  - Avaliação de 1 a 5 estrelas
  - Imagem da capa (redimensionada automaticamente)
  - Personagem favorito
- **Filtro por coleção** e contagem de fichas com nota média.
- **Contas individuais:** cada pessoa cria seu login e tem a própria estante, privada e separada das demais.
- **Sincronização entre dispositivos:** entre com o mesmo e-mail e senha em qualquer computador ou celular e suas fichas estarão lá.

---

## 🛠️ Tecnologias

- **HTML, CSS e JavaScript** puro (sem framework, sem etapa de build) — é um único arquivo `index.html`.
- **[Supabase](https://supabase.com/)** como backend: banco de dados PostgreSQL, autenticação por e-mail/senha e regras de segurança (Row Level Security) que isolam os dados de cada usuário.
- **[GitHub Pages](https://pages.github.com/)** para hospedagem gratuita.

---

## 🔒 Privacidade e segurança

Os dados de cada usuário ficam protegidos por políticas de Row Level Security (RLS) no Supabase: cada conta só consegue ler e editar as próprias fichas. A chave pública (*publishable key*) presente no código é segura para ficar exposta — é projetada exatamente para uso no navegador, e quem protege os dados são as regras de RLS, não o sigilo da chave.

---

---

Feito com carinho 🌸

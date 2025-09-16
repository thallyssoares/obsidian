> [!quote] "Um sistema de organização só funciona quando reflete a forma como você pensa."
> ---

---

## 🧠 Minha Filosofia de Uso

>[!info] Este é o manual do meu cérebro digital. Ele segue o método PARA para transformar caos em clareza.

#### 1. Projetos
- **O que são para mim:** _(Escreva com suas palavras. Ex: "São meus esforços ativos com começo, meio e fim. Cursos com prazo, trabalhos da faculdade, etc. É aqui que a 'ação' acontece.")_
- **Quando usar:** _(Ex: "Quando inicio um novo curso ou recebo um novo trabalho da faculdade.")_

#### 2. Áreas
- **O que são para mim:** _(Ex: "São as grandes áreas da minha vida que eu gerencio continuamente. Saúde, Finanças, Faculdade (como um todo), Desenvolvimento Pessoal. Não têm um 'fim'.")_
- **Quando usar:** _(Ex: "Para guardar meus planejamentos semanais, metas anuais, e anotações sobre hábitos.")_

#### 3. Recursos
- **O que são para mim:** _(Ex: "Minha biblioteca pessoal, minha 'despensa'. Aqui fica o conhecimento puro e atemporal sobre os tópicos que me interessam: Python, SQL, Idiomas, etc.")_
- **Quando usar:** _(Ex: "Após sintetizar uma nota de aula ou aprender algo novo, eu crio uma nota permanente aqui.")_

#### 4. Arquivo
- **O que é para mim:** _(Ex: "O cemitério de itens inativos. Projetos concluídos e áreas que não são mais relevantes vêm para cá para manter o sistema limpo.")_
- **Quando usar:** _(Ex: "Ao final de cada semestre ou quando concluo um grande projeto.")_

---

## 🎯 Projetos Ativos Atualmente

```dataview
TABLE dateformat(file.ctime, "dd/MM/yyyy") AS "Data de Início"
FROM "1. Projetos"
WHERE file.folder != "1. Projetos"
SORT file.ctime DESC
´´´
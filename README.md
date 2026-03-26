# Git em Equipe (Java) — README

Mini–projeto para treinar **Git em equipe (3 pessoas)** com Java. 
Cada pessoa implementa uma parte da classe `Calc` em **branches** diferentes, abre **Pull Requests** e resolve **um conflito de merge** intencional no `README.md`.

---

## 🎯 Objetivos de aprendizado
- Clonar repositório, criar branch, commit, push e abrir **PR**  
- Fazer **code review** e realizar **merge**   
- **Sincronizar** sua branch com `main` e **resolver conflitos** 

---

## ✅ Pré-requisitos
- Git instalado  
- Java 17+ (ideal 21)  
- Maven instalado (ou use sua IDE preferida)  
- Um repositório GitHub com **acesso de escrita** para as 3 pessoas

---

## 🔀 Fluxo de trabalho recomendado
- Uma branch por tarefa: `feature/soma`, `feature/subtracao`, `feature/multiplicacao`  
- Commits pequenos e mensagens claras (`feat: implementar soma`)  
- Abrir **PR** e solicitar **review** de pelo menos 1 colega  
- **Todos editam a MESMA LINHA** do `README.md` (abaixo) para forçar **conflito**

---

## 👤 Configuração de identidade (cada um, uma única vez)
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"
```
---

## 🧪 Como rodar
```bash
mvn -q -DskipTests package
java -cp target/git-equipe-java-1.0.0.jar equipe.Main
```

Saída esperada ao final (com tudo implementado):
```
2 + 3 = 5
3 - 2 = 1
2 * 3 = 6
```

---

## 👩‍💻 Status da Equipe

**Linha da equipe (edite ESTA MESMA LINHA para criar conflito): Equipe = [Victor Henrique Dias, Lucas Ferreira Andrade, Paulo Victor]**

---

## 📝 Dicas Úteis
### Git

- Status: `git status`  
- Histórico: `git log --oneline --graph --decorate --all`  
- Trazer `main` para sua branch (rebase):
  ```bash
  git fetch origin
  git pull --rebase origin main
  ```
- Desfazer último commit mantendo alterações: `git reset --soft HEAD~1`  
- Guardar alterações temporariamente: `git stash` / `git stash pop`

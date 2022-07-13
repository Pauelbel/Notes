# Основные команды

git config --global user.name "your_github_username"
git config --global user.email "your_github_email"

- Кэшировать УД
``` git config --global credential.helper cache``` 
- Удалить из кэша
``` git config --global --unset credential.helper```
``` git config --system --unset credential.helper ```
``` git config --global credential.helper cache ```
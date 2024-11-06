1. Клонируйте репозиторий:
  git clone --recurse-submodules https://github.com/IvanAngoldt/project-orchestration.git

2. Как запушить изменения в подмодуль (например, в фронтенде или бэкенде):
  Для фронтенда: cd frontend
  Для бэкенда: cd backend
  git add .
  git commit -m "Description of the changes"
  git push origin master

3. Как зафиксировать изменения в основном репозитории (project-orchestration)
  cd ..
  git submodule status
  git add .
  git commit -m "Update submodules (frontend and/or backend)"
  git push origin master

4. Как получить новшества на другом компьютере
  git pull origin master
  git submodule update --init --recursive
  git submodule status

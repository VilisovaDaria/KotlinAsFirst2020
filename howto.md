форк проекта KotlinAsFirst2020; 

git clone https://github.com/VilisovaDaria/KotlinAsFirst2020.git;

git remote add upstream-my https://github.com/VilisovaDaria/KotlinAsFirst2021.git;

git fetch upstream-my;

git rebase --onto master 43335d77 upstream-my/master (последний коммит до моих коммитов);

CONFLICT (content): Merge conflict in src/lesson2/task1/IfElse.kt;

git checkout 8eb7545f src/lesson2/task1/IfElse.kt;

git add src/lesson2/task1/IfElse.kt;

git rebase --continue;

git branch backport;

git checkout master;

git merge backport;

git remote add upstream-theirs https://github.com/FAbrickA/KotlinAsFirst2021;

git fetch upstream-theirs;

git merge -s ours upstream-theirs/master;

git remote -v > remotes;

git add remotes;

git commit -m "Add remotes file";

создаю файл - howto.md;

git add howto.md;

git commit -m "Add howto.md";

загружаю на github;

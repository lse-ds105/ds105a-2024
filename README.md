# LSE DS105A 2024/25

A repository for all the lecture and class materials used in the Autumn Term edition of DS105A (2024/25) at LSE


## How to fork this repository?

1. Click on the `Fork` button on the top right corner of this page.

2. You'll be redirected to your own forked repository.

3. Now, you can clone this repository to your local machine and start working on it.

## How to bring the changes from the original repository to your forked repository?

There are two options to do this, and it will depend on whether you have made changes to your forked repository or not.

### Option 1: You haven't made any changes to your forked repository

(Or you have made changes but you don't care about losing them)

1. Go to your forked repository on GitHub. You will see a message 'This branch is X commits behind lse-ds105/ds105a-2024:main'.

2. Click on the **'Sync Fork'** button.

3. Click on the **'Update branch'** button.

4. You will see a message 'This branch is up to date with lse-ds105/ds105a-2024:main'. Done!

### Option 2: If you want to keep the changes in your forked repository

(You've made changes and you want to keep them)

1. On your local machine, instruct Git that there is a remote repository called `upstream` that points to the original repository.

```bash
git remote add upstream git@github.com:lse-ds105/ds105a-2024.git
```

2. Instruct git to take a look at the changes in the original repository.

```bash
git fetch upstream/main
```

3. Merge the changes from the original repository to your forked repository.

```bash
git merge upstream/main
```

This might lead to [git conflicts](https://docs.github.com/en/github/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts) if you have made changes to the same files in your forked repository. You will need to resolve these conflicts manually. Ask any instructors for help if you're not sure how to do this.

4. Push the changes to your forked repository.

```bash
git push origin main
```

or simply

```bash
git push
```

(as by default, your forked repository is the origin)

5. Done!




# Revert Changes
Hopefully you have not forgotten about your assignment from the last chapter. But who wants to do an assignment? (Not me at least.) Luckily, you have a friend who has already done it. Let's copy his assignment,

    bool CopiedIsPrime(int n)
    {
        for (int i = 2; i < n; ++i)
        {
            if (n % i == 0)
                return false;
        }
        return true;
    }

Paste this function just before `int main()`. Commit your changes,

    $ git commit prime.cpp -m 'Borrowed IsPrime() from a friend (don't tell the teacher)'

> Note that `git add` is not required here since we are explicitly mentioning the name of the file we want to commit.

That's it. An assignment well done!

Well, not quite...
Unfortunately for you, your teacher is also a frequent visitor of GitHub and he sees your commit message. Now he is really angry. He screams, "Either you do it yourself or I will fail you." So you type,

    $ git reflog

> `4c29248 HEAD@{0}: commit: Borrowed IsPrime() from a friend (don't tell the teach
974dbe5 HEAD@{1}: commit (initial): First version`
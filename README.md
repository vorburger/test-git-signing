# test-git-signing

Testing signing my Git commits:

    git log --show-signature


if `KEYID` is your GPG Key ID, then enable this with:

    git config --global user.signingkey $KEYID
    git config --global commit.gpgsign true
    git config --global tag.forceSignAnnotated true

    gpg --armor --export $KEYID

and copy/paste that into https://github.com/settings/keys.

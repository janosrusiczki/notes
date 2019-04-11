Convert tabs to spaces

    :set tabstop=2 shiftwidth=2 expandtab
    :retab

Search and replace:

    :%s/foo/bar/g
    :%s/fOo/bAr/gI

Convert DOS line endings:

    :%s/\r//g

Remove trailing whitespaces:

    :%s/\s\+$//e

To check use a specific repo for commands

`yum --disablerepo="*" --enablerepo="foo" update`

To yum update with an exclusion for conflicts

`yum update --exclude=PACKAGENAME`

# NAME

Dist::Zilla::Plugin::ContributorCovenant - Add Contributor Covenant as Code of Conduct

# DESCRIPTION

`Dist::Zilla::Plugin::ContributorCovenant` adds the Contributor
Covenant to your CPAN build as `CODE_OF_CONDUCT.md`. It pulls
email address of first author from `dist.ini`. If none found,
it will type "GitHub / RT" instead.

# SYNOPSIS

Add this one line to your dist.ini.

    [ContributorCovenant]

If you want to leave a copy of Code Of Conduct in code repository,
You can add following lines to your dist.ini as well.

    [CopyFilesFromBuild]
    copy = CODE_OF_CONDUCT.md

Note that this plugin will prune other CODE\_OF\_CONDUCT.md files, to
avoid multiple CODE\_OF\_CONDUCT.md preventing the build.

The version of this module will match the version of the Contributor
Covenant used.  For instance, version 1.004001 will use Contributor
Covenant version 1.4.1.

# AUTHOR

Kivanc Yazan `<kyzn at cpan.org>`

# CONTRIBUTORS

Joelle Maslak `<jmaslak at antelope.net>`
D Ruth Holloway `<ruth at hiruthie.me>`

# COPYRIGHT AND LICENSE

This software is copyright (c) 2020 by Kivanc Yazan.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.

# ATTRIBUTION

\- This module is based heavily on [Dist::Zilla::Plugin::Covenant](https://metacpan.org/pod/Dist::Zilla::Plugin::Covenant).

\- Covenant text is taken from [https://www.contributor-covenant.org/version/2/0/code\_of\_conduct/code\_of\_conduct.md](https://www.contributor-covenant.org/version/2/0/code_of_conduct/code_of_conduct.md).

# SEE ALSO

\- Contributor Covenant, [https://www.contributor-covenant.org/](https://www.contributor-covenant.org/)

\- VM Brasseur's "The Importance of Ecosystem" Keynote, [https://archive.org/details/yatpc2018-ecosystem](https://archive.org/details/yatpc2018-ecosystem)

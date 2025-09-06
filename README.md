# Bash with Style
#### _(an opinionated bash scripting styleguide crafted over 20 years)_

----
# Introduction

The following is an opinionated styleguide for bash scripts, written after 20+
years of bash scripting. Where relevant, justification for each guideline is
detailed.

It is licensed under the _Creative Commons Attribution 4.0 International
license_. For more information, see [LICENSE](LICENSE) / [COPYING](COPYING) or
visit https://creativecommons.org/licenses/by/4.0/ .

For a list of the main author(s), and other contributors, see
[AUTHORS](AUTHORS.md) and [CONTRIBUTORS](CONTRIBUTORS.md) respectively.

For more information on contributing (new feature, bug fix, pull request etc),
please see [CONTRIBUTING](CONTRIBUTING.md) .

----
# Table of Contents

{:toc}

----
# Background

## What this styleguide is and isn't

### Shell scripting guide?

This styleguide is specifically for `bash` scripts, not (Bourne) shell scripts,
`dash`, `ksh`, `csh`, `fish` or any other variant.

### Bash versions

Whilst most of this applies to older versions of `bash`, some items may not be
compatible with _EXTREMELY_ old `bash` (eg. 20 years+). This will mainly impact
much older installations and Apple Mac OS users (who haven't updated their
`bash` from the 20 year old one that is shipped with their system).

Where possible (and known) version discrepancies/dependencies will be
documented.

### External components

A lot of the power of shell scripts like Bash, is calling out to other helper
programs. Therefore, this styleguide will also include references to those tools
and how they are used within the `bash` scripts. As with Bash version
compatibility, where possible (and known) any version discrepancies with these
tools will be documented, and where possible alternatives provided.

Most of the tools used are from the GNU Coreutils package such as: `tr`, `cut`,
     `head`, `tail`, `cat`, `tac`, `sort`, `uniq`, `wc`, `stat`, `seq`,
     `dirname`, `readlink`, `realpath`, `mktemp`, `mkfifo`, `mkdir`, `rmdir`,
     `rm`, `du`, `df`, `date`, `chmod`, `chown`, `chgrp`, `basename`, `base64`,
     `md5sum` and `sha256sum`.

Others such as `printf` and `echo` are `bash` builtins.

GNU `sed` is also utilised.

----
[//]: # ( vim: set ts=4 sw=4 et cindent tw=80 ai si syn=markdown ft=markdown: )

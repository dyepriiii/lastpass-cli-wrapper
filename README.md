# Intro

This is an attempt at learning Perl by creating a lastpass-cli interface/wrapper

# Starting

Copy `config_sample` to `config`

# Usage

```
Usage
  ./lp [ --help | -h | -? ] to show this message
  ./lp [ --add | --new | -a | -n ]
  ./lp [ --rm | --delete | -r | -d ] ID1 {ID2 ID3 ...}
  ./lp [ --search | -s ] SEARCH_QUERY
  ./lp [--edit | -e ] NAME_OR_ID
```

# Notes
 - Currenly entries are only `server` secure note (useful for storing 
   server login details)
 - `--add` option will ask for user/pw/hostname/entryname etc
 - if password is empty, one generated for you (via lastpass)
 - `--delete` can take multiple ids/name, just qoute them:
   `lp -d "791285516313975075 8249657000128659549 9118066746859183309"`

# Requirements
 - lastpass-cli (>= 1.0)
 - cpan modules
     - String::ShellQuote
     - - Getopt::Long

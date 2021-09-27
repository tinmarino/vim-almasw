Vim plugin to facilitate Alma software navigation

# Quickstart

```bash
cd .vim
git submodule add https://github.com/tinmarino/vim-almasw pack/bundle/opt/almasw
```

```vim
packadd almasw
```

# Features

* Enhanced `gf` with `&path` variable


# Util

```bash
#rsync -av \
#  --exclude="/ACSSW-*/" \
#  --exclude="/acsdata-*/" \
#  --exclude="/ACSSW/" \
#  --include="/TAO/" \
#  almamgr@acse2-gns.sco.alma.cl:/alma/ACS-current/ /home/tourneboeuf/Program/ACS-current
#  #--include="ACSSW/include" \
#  #--include="ACSSW/idl" \
#  #--include="ACSSW/Sources" \

#  find | rg '(.*)\.([^./]*)$' -r '$2' | sed 's/ //g' | sort | uniq -c | sort -n

rsync -av \
  --exclude="/ACSSW*/" \
  --exclude="/acsdata*/" \
  --include="*/" \
  --include="*.idl" \
  --include="*.h" \
  --include="*.inl" \
  --include="*.cpp" \
  --include="*.cc" \
  --include="*.java" \
  --include="*.py" \
  --include="*.css" \
  --include="*.js" \
  --include="*.xsd" \
  --include="*.xml" \
  --include="*.conf" \
  --include="*.txt" \
  --exclude="*" \
  almamgr@acse2-gns.sco.alma.cl:/alma/ACS-current/ /home/tourneboeuf/Program/ACS-current
```

# References

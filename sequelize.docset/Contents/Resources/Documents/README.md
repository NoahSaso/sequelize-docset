# sequelize-docset

Generated docset based on [https://sequelize.org/master/identifiers.html](https://sequelize.org/master/identifiers.html)

For use in apps such as [Dash](https://kapeli.com/dash)

## How to Build

```
# Install docset-from-HTML generator (dashing)
brew install dashing

# Download ESDoc-generated site
wget \
  --recursive \
  --no-clobber \
  --page-requisites \
  --html-extension \
  --convert-links \
  --domains sequelize.org \
  --no-parent \
      https://sequelize.org/master/identifiers.html

# Create docset (ensuring dashing.json is present)
dashing build sequelize
```

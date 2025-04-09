# create a new site in the root folder, force it because it's not empty
hugo new site . --force

# add ananke theme
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke

# set theme
echo 'theme = "ananke"' >> config.toml

# create new post
hugo new posts/my-first-post.md

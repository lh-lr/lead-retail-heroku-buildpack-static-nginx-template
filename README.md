# Heroku NGINX configurtaion template override

This buildpack allows overriding of the NGINX configuration template used by the buildpack  [heroku-buildpack-static](https://github.com/heroku/heroku-buildpack-static).

## Usage

1. Create template file in path `nginx/config/templates/nginx.conf.erb`
2. Add the buildpack right after the heroku-buildpack-static position as shown:

```bash
❯ heroku buildpacks -a app-name
=== app-name Buildpack URLs
1. https://github.com/debitoor/ssh-private-key-buildpack.git
2. https://github.com/mars/create-react-app-buildpack.git
3. https://github.com/dempj/heroku-buildpack-nginx-template.git
```
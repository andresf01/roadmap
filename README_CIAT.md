1 - Clone repository
2 - Checkout run branch
3 - `rvm use 2.4.4`
4 - Follow installation guidelines (wiki) Icluding static files (lib)
5 - Run mysql
6 - Install imagemagick `$ sudo apt install imagemagick`
7 - Setup devise.rb (ORCID)
8 - ORCID URI Redirect: domain.com/users/auth/orcid
9 - Run `$ rails s -b $IP -p $PORT` for development environment
10 - Run `$ rails s -e production -b $IP -p $PORT` for production environment

NOTES
- In development environment fies application css and js, and vendor.js are named like vendor-HASH.js where HASH is taking into account in production but not in development mode
- In production for rails serve public files code `config.serve_static_files = true` and `config.serve_static_assets = true`
- For running from terminal `$ nohup rails s -b $IP -p $PORT > /dev/null &`
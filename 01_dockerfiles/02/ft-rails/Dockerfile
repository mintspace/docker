FROM ruby

RUN apt-get update -y && apt-get install -y build-essential libpq-dev nodejs sqlite3

ONBUILD COPY app /opt/app
ONBUILD WORKDIR /opt/app

ONBUILD EXPOSE 3000
ONBUILD RUN bundle install
ONBUILD RUN rake db:migrate
ONBUILD RUN rake db:seed

# git clone https://bitbucket.org/railstutorial/sample_app_4th_ed.git app
# rake 12.2.1 -> 12.2.2 
# docker build -t ft_rails:on-build .

# eval $(docker-machine env Char) 

# e1z2r7p24% vboxmanage modifyvm Char --cpus=4
# e1z2r7p24% vboxmanage modifyvm Char --memory=8000

# docker run -it --rm -p 3000:3000 ex02

# http://192.168.99.100:3000
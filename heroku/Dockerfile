 from    git.bonustab.net:5050/bonustab/buildstep
 run     apt-get install wget -y --force-yes
 run     wget http://github.com/g00d-guy/basebuilder/tarball/master -O basebuilder.tar.gz --no-check-certificate
 run     mkdir /var/lib/tsuru
 run     tar -xvf basebuilder.tar.gz -C /var/lib/tsuru --strip 1
 add     deploy /var/lib/tsuru/deploy
 run     chmod +x /var/lib/tsuru/deploy
 run     cp /var/lib/tsuru/base/restart /var/lib/tsuru
 run     cp /var/lib/tsuru/base/start /var/lib/tsuru
 run     /var/lib/tsuru/base/install
 run     /var/lib/tsuru/base/setup
 add     circus.ini /etc/circus/circus.ini

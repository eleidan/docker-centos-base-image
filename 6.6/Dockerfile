FROM centos:6.6

LABEL maintainer="Oleg Kulyk" \
      description="CentOS 6.6" \
      run="docker run -it --rm -v $(pwd):/home/phantom/app eleidan/centos:6.6" \
      version="2017-08-01"

ENV HOME="/root" \
    SERVICE_NAME="centos:6.6" \
    CONTAINER_PS1="[ $(get_container_ip) | \[\e[0;36m\]$(get_container_service)\[\e[m\] | \[\e[0;35m\]\w\[\e[m\] ]\n\[\e[1;32m\]>\[\e[m\] "

COPY .profile .bashrc .bash_history  /etc/skel/
COPY .profile .bashrc .bash_history  $HOME/

CMD ["/bin/bash"]

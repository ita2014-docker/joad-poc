# BASE chef/ubuntu-12.04:latest
FROM joad/ci
ADD chef/ /etc/chef/
RUN chef-init --bootstrap
RUN rm -rf /etc/chef/secure/*
ENTRYPOINT ["chef-init"]
CMD ["--onboot"]

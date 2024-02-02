FROM base

MAINTAINER Ivan Ermilov <ivan.s.ermilov@gmail.com>

HEALTHCHECK CMD curl -f http://localhost:9870/ || exit 1

ENV HDFS_CONF_dfs_namenode_name_dir=file:///hadoop/dfs/name
RUN mkdir -p /hadoop/dfs/name
VOLUME /hadoop/dfs/name

EXPOSE 9870

# install jupyter notebook
RUN pip install jupyterlab
EXPOSE 8888

# DATA SCIENCE INSTALLS
RUN pip install opendatasets pandas scikit-learn matplotlib seaborn

#BIG DATA INSTALLS
RUN pip install hdfs mrjob
EXPOSE 4040

#MONGODB INSTALLS
RUN pip install pymongo

ADD run.sh /run.sh
RUN chmod a+x /run.sh
CMD ["/run.sh"]

FROM websphere-liberty
COPY /mc-web-test/server.xml /opt/ibm/wlp/usr/servers/defaultServer/server.xml 
COPY /mc-web-test/target/mc-web-test.war /opt/ibm/wlp/usr/shared/apps/mc-web-test.war
ENV LOG_DIR /logs
ENV WLP_OUTPUT_DIR /opt/ibm/wlp/output
RUN ln -s $WLP_OUTPUT_DIR/defaultServer /output \
    && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config

EXPOSE 22


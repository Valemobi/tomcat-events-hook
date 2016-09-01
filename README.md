# Event Hook Listener
Simple component to hook up scripts to Tomcat's Lifecycle events.

## Installation
- Build the jar using AND (`ant jar`)
- Put the tomcat-events-hook.jar in Tomcat's classpath
- Reference the listener in `${TOMCAT_HOME}/conf/server.xml` (`<Listener className="br.com.valemobi.tomcat.EventHookListener" />`)
- Start Catalina with the variable TOMCAT_POST_INIT_SCRIPT (like `TOMCAT_POST_INIT_SCRIPT=/path/to/post.init.sh ${TOMCAT_HOME}/bin/catalina.sh start`)
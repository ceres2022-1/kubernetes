# kubernetes
## liveness and readiness
Para agregar estos dos nuevos endpoints en el proyecto de springboot se modificó la libs del proyecto y la configuración.

Nueva dependencia 

`<dependency>
			<groupId>org.springframework.boot</groupId>
   			 <artifactId>spring-boot-starter-actuator</artifactId>
		</dependency>`

Y luego en el properties

* management.endpoint.health.probes.enabled=true
* management.health.livenessState.enabled=true
* management.health.readinessState.enabled=tru
# Configure hosts file C:\Windows\System32\drivers\etc liek below:
127.0.0.1       localhost
127.0.0.1       config
127.0.0.1  		auth-service
127.0.0.1  		auth-mongodb
127.0.0.1 		registry
127.0.0.1		account-mongodb
127.0.0.1		account-service
127.0.0.1		rabbitmq
127.0.0.1		notification-mongodb
127.0.0.1		statistics-mongodb

#02) modify configuration files
 	config/src/main/resources/shared/account-service.yml
	config/src/main/resources/shared/auth-service.yml
	config/src/main/resources/shared/monitoring.yml
	config/src/main/resources/shared/notification-service.yml
	config/src/main/resources/shared/statistics-service.yml
	config/src/main/resources/shared/turbine-stream-service.yml

	
#)
http://localhost:4000/

http://localhost:8989/hystrix-dashboard

#) hystrix dashboard
http://localhost:8080/hystrix

#turbine stream
http://localhost:8989/turbine/turbine.stream
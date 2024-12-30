Software Documentation
Software Name: Banking Application
Version: v1.0.0
1. Overview
The Banking Application is a backend service designed to handle banking operations. It uses Spring Boot for the core application, PostgreSQL for data storage, Kafka for messaging, and NGINX as a reverse proxy.

2. API Documentation
Base URL: http://localhost:8090
http://localhost:8090



3. Testing
Running Tests
To run the unit tests, use the following command:
bash
Copy code
./mvnw test
Test Coverage
JUnit 5 is used for unit testing.
Mockito is used for mocking dependencies in tests.

java
Copy code
@ExtendWith(MockitoExtension.class)
public class AccountServiceTest {

    @Mock
    private AccountRepository accountRepository;

    @InjectMocks
    private AccountService accountService;

   
}
4. Release Notes
Version 1.0.0
Initial release.
Basic banking operations supported:
Account creation
Balance retrieval
Fund transfer


The  application is not full implemented and does not have a frontend. Work in progress for the frontend and other backend features.





Spring resources versioning issue
=================================

Steps to reproduce the issue https://github.com/spring-projects/spring-framework/issues/26382
1. Run the application with `./mvnw spring-boot:run`
2. Visit http://localhost:8080. Yo should see a message in green.
3. Change the color of the message in `theme.css`
4. Hit <kbd>F5</kbd> (refresh the page). You should see the message in other color. What you got instead is the same result as before (cached by the browser).
4. Hit <kbd>Ctrl</kbd>+<kbd>F5</kbd> (refresh without cache). Now the message should be styled correctly.
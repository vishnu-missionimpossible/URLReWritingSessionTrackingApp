# URLReWritingSessionTrackingApp

1. In the Cookie session tracking mechanism,  if client doesn't allow cookies then our application won't work properly same case applies to HttpSession tracking mechansim as well because internally it uses cookie to store session id.
2. To overcome this problem we will go for URL ReWriting session tracking approach where we no need to depend neither on the client side nor on the server side. 
4. Using response.encodeURL() method, we will attach the session id in the URL itself 
5. In the previous project(HttpSession tracking and CookieSession Tracking) we have created static pages but here we will create dynamic forms to provide more stable application.
6. In the Firsrt servlet, we will get the data from the index.html using request object and we will store that information in session object and then we will create a dynamic form uing PrintWriter object and response object and that form will be linked to the second servlet.
7. In the second servlet we will get the data from the form present in the First Servlet and then we will store it in the session object and then we will create a dynamic form uing PrintWriter object and response object and that form will be linked to the third servlet.
8. In the third servlet we will get the data from the form present in second servlet and we will get the data from the session object and then  we will create a printWriter object uing response object and then we will display the result.

Note: Static html page if we use means we cannnot attach the session Id in the URL. It is only possible when we use dynamic forms. 

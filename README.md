# Testing APIs with Postman

## Learning Goals

- Review how to use Postman.

## Review Using Postman

In the previous module, we learned how to use a tool called Postman as an API
client when testing our servlets. We can use the same tool here too to test our
Spring web applications!

So far, we've only created a controller class with `GET` requests, so we can
easily test these in a browser's URL bar. But when we start introducing some other
HTTP verbs, like `POST`, `PATCH`, and `DELETE`, it will be easier to use an API
client, like Postman.

Even though we haven't introduced these other HTTP verbs yet in our controller
class, let's do a quick refresh on how we can test our application using one of
the `GET` requests we have defined.

In our spring-web-demo project, open up the `LunchController` class. Let's test
with the `getLunchSpecial()` method! Run the `SpringWebDemoApplication` and then
open up Postman, which should have already been installed from the previous
module.

Once Postman is opened up, enter in HTTP request mapped to the `getLunchSpecial()`
method in the controller class. Let's use `monday` as the path variable, so the
`GET` request should be "http://localhost:8080/lunch-special/monday".

![postman-lunch-query](https://curriculum-content.s3.amazonaws.com/spring-mod-1/postman/postman-lunch-special-query.png)

Let's see if this works now! Click the "Send" button next to the request.

![postman-lunch-result](https://curriculum-content.s3.amazonaws.com/spring-mod-1/postman/postman-lunch-special-result.png)

Looks like the lunch special on Monday is a BLT sandwich! Yippee! Looks like
everything works. We'll continue to use Postman as a testing tool. Now let's get
into debugging our application.

## Conclusion

API clients like Postman are extremely valuable to have in your API developer
toolkit. They make it simple to interact with servers by giving you full control
over how the response is being sent, with a nice interface for customizing the
HTTP verb, URL, headers, and body.

In future lessons, we'll be expanding our API to handle non-GET requests, so
being able to use a tool like Postman will make our API development much easier!
It's also a great tool to use if you're exploring a third-party API for use in
your projects.

## Resources

- [Postman Documentation](https://learning.postman.com/docs/getting-started/sending-the-first-request/)

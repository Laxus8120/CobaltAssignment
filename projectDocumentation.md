# Cobalt Assisment(Backend Developer Internship)

 <details close>
 <summary><h1>What is OAuth ?</h1></summary>

**Roles**

   ***OAuth defines four roles:***

*resource owner

      An entity capable of granting access to a protected resource.
      When the resource owner is a person, it is referred to as an
      end-user.

*resource server
      The server hosting the protected resources, capable of accepting
      and responding to protected resource requests using access tokens.

*client
      An application making protected resource requests on behalf of the
      resource owner and with its authorization.  The term "client" does
      not imply any particular implementation characteristics (e.g.,
      whether the application executes on a server, a desktop, or other
      devices).

*authorization server
      The server issuing access tokens to the client after successfully
      authenticating the resource owner and obtaining authorization.

>NOTE - The interaction between the authorization server and resource server
   is beyond the scope of this specification.  The authorization server
   may be the same server as the resource server or a separate entity.
   A single authorization server may issue access tokens accepted by
   multiple resource servers.

Protocol Flow

     +--------+                               +---------------+
     |        |--(A)- Authorization Request ->|   Resource    |
     |        |                               |     Owner     |
     |        |<-(B)-- Authorization Grant ---|               |
     |        |                               +---------------+
     |        |
     |        |                               +---------------+
     |        |--(C)-- Authorization Grant -->| Authorization |
     | Client |                               |     Server    |
     |        |<-(D)----- Access Token -------|               |
     |        |                               +---------------+
     |        |
     |        |                               +---------------+
     |        |--(E)----- Access Token ------>|    Resource   |
     |        |                               |     Server    |
     |        |<-(F)--- Protected Resource ---|               |
     +--------+                               +---------------+
</details>
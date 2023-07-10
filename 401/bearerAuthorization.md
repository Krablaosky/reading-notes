# Intro to JWT

1. [What is a JSON Web Token (JWT)?](https://jwt.io/introduction/)

  A JSON Web Token (JWT) is a standardized format for securely transmitting information between parties as a JSON object. It consists of three main parts: a header, a payload, and a signature. The header contains information about the type of token and the cryptographic algorithm used to sign it. The payload contains the claims or statements about the user or entity, such as their identity or authorization data. The signature is used to verify the integrity of the token and ensure that it has not been tampered with.

2. When should we use JSON Web Tokens?

  JSON Web Tokens can be used in various scenarios where secure transmission and authentication of information are required. Some common use cases include:

  Authentication: JWTs can be used to verify the identity of users during the authentication process. They can contain claims such as user ID, roles, or permissions, which can be used to determine the user's access rights.

  Authorization: JWTs can be used to authorize access to specific resources or functionalities. The claims within the token can be checked to ensure that the user has the necessary permissions.

  Single Sign-On (SSO): JWTs can be used in SSO systems to allow users to authenticate once and access multiple applications or services without the need to re-enter credentials.

  Information Exchange: JWTs can be used to securely exchange information between different parties in a distributed system. The token can carry relevant data and assertions, providing a trusted means of communication.

3. Claims are expected in which structural component of a JWT?

  Claims are expected in the payload component of a JWT. The payload is a JSON object that contains the claims or statements being made about the user or entity. These claims can include information such as user ID, roles, permissions, or any other relevant data that needs to be transmitted or verified.

## [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

1. If I get a JWT and I can decode the payload, how can we call that secure?

  If you can decode the payload of a JWT, it does not necessarily mean that the JWT is insecure. JWTs use a digital signature to ensure the integrity and authenticity of the token. Decoding the payload only allows you to view the information contained within the token. However, to modify the token or create a valid signature, you would need the secret key used to sign the token. Without the secret key, you cannot tamper with the token or create a valid signature, which helps maintain the security of the JWT.

2. If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

  When sending a JWT, both the sender and receiver must know the secret key used to sign the token. The secret key is a shared secret between the parties involved. The sender signs the JWT using the secret key, and the receiver can verify the signature using the same secret key. This ensures that the JWT has not been tampered with during transmission and provides a means of trust between the parties.

3. Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.
Videos

  To securely send concatenated content and a secret to a non-technical recruiter, you can follow these steps:

   * Use a secure communication channel: Ensure that the communication channel you are using to send the content and secret is secure. For example, you can use encrypted email, a secure file-sharing platform, or a secure messaging application.

   * Encrypt the content: Encrypt the concatenated content using a strong encryption algorithm. This ensures that even if the information is intercepted, it remains unreadable to unauthorized individuals. Provide the non-technical recruiter with the necessary instructions or password to decrypt the content.

    *  Share the secret separately: Send the secret (e.g., the secret key for signing a JWT) through a separate secure channel. This could be a different encrypted message, a phone call, or an in-person meeting. Emphasize the importance of keeping the secret confidential and not sharing it with anyone else.

  By following these steps, you can ensure that both the concatenated content and the secret are transmitted securely to the non-technical recruiter, minimizing the risk of unauthorized access or tampering.

## [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)

1. Why use JWT?

  JWTs are used for authentication and authorization in web applications and APIs. They are stateless, simplify authorization, offer flexibility, and provide security through digital signatures.

2. JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

  Imagine carrying important documents in a compact envelope instead of a folder. Similarly, JWTs contain all relevant information in a compact and self-contained manner. The header describes the algorithm, the payload includes claims, and the signature ensures integrity. This makes JWTs efficient to transmit, validate, and understand.

3. What are the three components (the structure) of a JWT signature?

  The JWT signature has three components:

  * Header: Describes the algorithm and token type.
  * Payload: Contains claims or statements about the user or entity.
  * Signature: Created using the encoded header, encoded payload, and a secret key. It verifies the token's authenticity and integrity.

## [Back](../401readingNotes.md)
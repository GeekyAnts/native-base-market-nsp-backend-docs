## User Collection Schema :

```  
email: { type: String, required: true },

password: { type: String, required: true, select: false  },

createdAt: {  type: Date,  default: Date.now  },

jwtAccessToken: {  type: String,  default: null  },

```


# Transaction-Management-in-SpringBoot using @Transactional(propogation=Propagation.Required)
Database transaction management in springboot: https://www.javainuse.com/spring/boot-transaction-propagation

### Propagation	Behaviour:
1) REQUIRED:	Always executes in a transaction. If there is any existing transaction it uses it. If none exists then only a new one is created
2) SUPPORTS:	It may or may not run in a transaction. If current transaction exists then it is supported. If none exists then gets executed with out transaction.
3) NOT_SUPPORTED:	Always executes without a transaction. If there is any existing transaction it gets suspended
4) REQUIRES_NEW:	Always executes in a new transaction. If there is any existing transaction it gets suspended
5) NEVER:	Always executes with out any transaction. It throws an exception if there is an existing transaction
6) MANDATORY:	Always executes in a transaction. If there is any existing transaction it is used. If there is no existing transaction it will throw an exception.

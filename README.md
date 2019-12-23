# CakePHP3 Plugin for Amazon Mail

## Amazon set-up
You need to have an Amazon SES account

## Steps to install

1. Copy the contents in /plugins/
2. Edit /config/app.php 
```
'EmailTransport' => [
  'amazon' =>  [
      'host' => 'email-smtp.eu-central-1.amazonaws.com',
      'port' => 587,
      'username' => 'USERNAME',
      'password' => 'PASSWORD',
      'className' => 'Smtp',
      'tls' => true
  ]
]
```

and here

```
'Email' => [

  ....
  
  'production' => [
    'transport' => 'amazon',
    //'log' => true,
  ]
  
  ...
  
]
```

3. 

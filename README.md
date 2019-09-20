# node-red-contrib-rotate-logger

This project is forked from [`Rotate Logger`](https://github.com/airkjh/node-red-contrib-advance-logger)

I chaged for support winston:3.2.1 and winston-daily-rotate-file:4.1.0 (2019-09-20)

to support a configuration similar to:

```
  var transport = new (winston.transports.DailyRotateFile)({
    filename: '/log/application-%DATE%.log',
    datePattern: 'YYYY-MM-DD-HH',
    zippedArchive: true,
    maxSize: '20m',
    maxFiles: '14d'
  });
```



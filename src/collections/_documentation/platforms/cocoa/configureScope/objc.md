```objc
[SentrySDK configureScope:^(SentryScope * _Nonnull scope) {
    [scope setEnvironment:@"debug"];
    [scope setTagValue:@"objc" forKey:@"langauge"];
    [scope setExtraValue:[NSString stringWithFormat:@"%@", self] forKey:@"currentViewController"];
}];
```
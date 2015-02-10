* Naming for protocol
```objc
@class EOCNetworkFetcher;
@protocol EOCNetworkFetcherDelegate <NSObject>
- (void)networkFetcher:(EOCNetworkFetcher*)networkFetcher didFinishWithData:(NSData*)data; 
@end
```

* Naming for typedef block
```objc
typedef void(^ACAccountStoreSaveCompletionHandler) (BOOL success, NSError *error);
typedef void(^ACAccountStoreRequestAccessCompletionHandler) (BOOL granted, NSError *error);
```

* Naming for method in category
```objc
+ (UIStoryboard *)tp_mainStoryboard;
```
* Naming for segue identifier
```objc
- (void)prepareForSegue:(UIStoryboardSegue *)segue sender:(id)sender {
    if ([segue.identifier isEqualToString:@"ShowRecipePhoto"]) {
    }
}
```
* Naming for Outlet
```objc
@property (weak, nonatomic) IBOutlet UIBarButtonItem *shareButton;
```

* Naming for IBAction
```objc
- (IBAction)shareButtonTouched:(id)sender;
```

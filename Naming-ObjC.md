

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


Return instead of using if else

```objc
[[TPUserManager sharedInstance] registerToMailingListWithEmail:self.emailTextField.text completionHandler:^(NSString *errorMessage) {
            if (errorMessage) {
                [SVProgressHUD showErrorWithStatus:errorMessage];
                return;
            }
            
            [SVProgressHUD dismiss];
            
            [[TPUserManager sharedInstance] LogOut];
            [self dismissViewControllerAnimated:YES completion:nil];
        }];
```

```objc
[[TPUserManager sharedInstance] registerToMailingListWithEmail:self.emailTextField.text completionHandler:^(NSString *errorMessage) {
            if (errorMessage) {
                [SVProgressHUD showErrorWithStatus:errorMessage];
            }
            else {
                [SVProgressHUD dismiss];
                
                [[TPUserManager sharedInstance] LogOut];
                [self dismissViewControllerAnimated:YES completion:nil];
            }
        }];
```

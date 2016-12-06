# GFCodeScan
The use of CAShappeLayer real-time capture of the scanned graphics, you can automatically scan and provide a return of the data interface；利用CAShappeLayer 实时捕捉扫描的图形，可以自动扫描并提供返回的数据接口

how to use it:
#import "GFCodeScanViewController.h"
 GFCodeScanViewController* scanVC = [[GFCodeScanViewController alloc]init];
    [scanVC getInfoWithDecodeBlock:^(NSString *text) {
        self.label.text = text;   
    }];
    [self.navigationController showViewController:scanVC sender:nil];
    

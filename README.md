# more-objects-lhp-1

#import <Foundation/Foundation.h>

int main(int argc, const char * argv[]) {
    @autoreleasepool {
        
        
        NSDateFormatter *formatter = [[NSDateFormatter alloc] init];
        NSString *dateFormat = @"yyyy-MM-dd";
        [formatter  setDateFormat: dateFormat];
        NSString *birthDate = @"1992-12-09";
        NSDate *birthday = [formatter dateFromString:birthDate];
        NSLog(@"%@", birthday);
        
        // OR...! vvvvv
        
        NSDateFormatter *formatter2 = [[NSDateFormatter alloc] init];
        formatter2.dateFormat = @"yyyy-MM-dd";
        NSDate *date = [formatter2 dateFromString:@"1992-12-09"];
        NSLog(@"%@", date);
        
        //NSLog(@"%@", formatter);
    
        
    }
    return 0;
}

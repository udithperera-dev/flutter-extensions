# flutter-extensions
Some of useful extension for manipulate text and data sets in flutter

Unique Extension(remove-duplicates.dart)
## Example for Value List:  

        List<int> list = [1,1,1,2,4,5,8,8];
        list.unique((x) => x);
        Output: [1,2,4,5,8]
        
## Example for Model List: 
        
        List<Man> manList = [
                              Man(name:'a',height: 2),
                              Man(name:'a',height: 2),
                              Man(name:'b',height: 3),
                              Man(name:'c',height: 2),
                              Man(name:'d',height: 5),
                              Man(name:'d',height: 2),
                            ];
        list.unique((x) => x.name);
        Output: [
                  Man(name:'a',height: 2),
                  Man(name:'b',height: 3),
                  Man(name:'c',height: 2),
                  Man(name:'d',height: 5)
                ]
                
                
                

        list.unique((x) => x.height);
        Output: [
                    Man(name:'a',height: 2),
                    Man(name:'b',height: 3),
                    Man(name:'d',height: 5)
                ]

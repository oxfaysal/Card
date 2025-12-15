# Card

### Design 1
```
Card(
              child: Padding(
                padding: EdgeInsets.all(8.0),
                child: SizedBox(
                  height: 100,
                  child: Row(
                    children: [
                      Container(
                        child: CircleAvatar(
                          backgroundImage: NetworkImage("https://avatars.githubusercontent.com/u/248434219"),
                          radius: 100,
                        ),
                        height: 60,
                        width: 60,
                      ),
                      Expanded(
                        child: Padding(
                          padding: EdgeInsetsGeometry.only(left: 10, right: 10),
                          child: Column(
                            mainAxisAlignment: MainAxisAlignment.center,
                            crossAxisAlignment: CrossAxisAlignment.start,
                            children: [Text("Faysal"), Text("Shariatpur, Dhaka")],
                          ),
                        ),
                      ),
                      Container(
                        child: IconButton(onPressed: () {}, icon: Icon(Icons.call)),
                      ),
                    ],
                  ),
                ),
              ),
            ),
```

#### Demo Image
<img src="https://i.ibb.co.com/PGqVKh8R/Screenshot-2025-12-15-073207.png" alt="Demo"></a>



###### © All right reserved by Faysal




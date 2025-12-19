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


### Design 2
```
Card(
          child: Container(
            height: 100,
            padding: EdgeInsets.all(10),
            child: Row(
              mainAxisAlignment: MainAxisAlignment.start,
              children: [
                Expanded(
                  flex: 2,
                  child: InkWell(
                      onTap: () => ScaffoldMessenger.of(context).showSnackBar(SnackBar(content: Text("My Image"))),
                      child: CircleAvatar(
                        radius: 30.0,
                        backgroundImage: NetworkImage("https://i.ibb.co.com/Zp43nK1M/1000058742-photoaidcom-2x-ai-zoom.png", ),
                        backgroundColor: Colors.transparent,
                      )),
                ),
                Spacer(),
                Expanded(
                  flex: 7,
                  child: Column(
                    crossAxisAlignment: CrossAxisAlignment.start,
                    mainAxisAlignment: MainAxisAlignment.center,
                    children: [
                      Text(
                        "Faysal",
                        style: TextStyle(fontSize: 20, color: Colors.indigo),
                      ),
                      Text(
                        "Dewan kandi, Shakhipur, Shariatpur",
                        style: TextStyle(fontSize: 14, color: Colors.black54),
                      ),
                    ],
                  ),
                ),
                Spacer(),
                Expanded(
                  flex: 1,
                  child: IconButton(onPressed: () {
                    ScaffoldMessenger.of(context).showSnackBar(SnackBar(content: Text("Call Now")));
                  }, icon: Icon(Icons.call)),
                ),
              ],
            ),
          ),
        ),

```

#### Demo Image
<img src="https://i.ibb.co.com/PGqVKh8R/Screenshot-2025-12-15-073207.png" alt="Demo"></a>






###### © All right reserved by Faysal




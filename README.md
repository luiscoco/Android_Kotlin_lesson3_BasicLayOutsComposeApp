# Learn Basic Layouts in Android Compose application 

https://developer.android.com/develop/ui/compose/layouts/basics

## 1. My first layout sample: Adding a Column with two Text components

![image](https://github.com/luiscoco/Android_Kotlin_lesson3_BasicLayOutsComposeApp/assets/32194879/abdfff75-490a-415e-ba26-b074ca0b7dab)

```kotlin
@Composable
fun ArtistCardColumn() {
    Column {
        Text("Alfred Sisley")
        Text("3 minutes ago")
    }
}
```

## 2. Using Row, Column and Text components

Use Row to place items horizontally on the screen. Both Column and Row support configuring the alignment of the elements they contain

![image](https://github.com/luiscoco/Android_Kotlin_lesson3_BasicLayOutsComposeApp/assets/32194879/4d43b7fc-58e3-4438-aaab-02ce62bc9ccd)

```kotlin
@Composable
fun ArtistCardRow(artist: Artist) {
    Row(verticalAlignment = Alignment.CenterVertically) {
        Image(bitmap = artist.image, contentDescription = "Artist image")
        Column {
            Text(artist.name)
            Text(artist.lastSeenOnline)
        }
    }
}
```

## 3. Using a Box

Use Box to put elements on top of another. Box also supports configuring specific alignment of the elements it contains.

![image](https://github.com/luiscoco/Android_Kotlin_lesson3_BasicLayOutsComposeApp/assets/32194879/25ad481d-1578-4585-aa67-897c9e8d8ed5)

```kotlin
@Composable
fun ArtistAvatar(artist: Artist) {
    Box {
        Image(bitmap = artist.image, contentDescription = "Artist image")
        Icon(Icons.Filled.Check, contentDescription = "Check mark")
    }
}
```

## 4. 



## 5. 

## 6. 

## 7. 



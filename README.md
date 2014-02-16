##Examples

### Old Way

```c++
// Header
class Object {
public:
  Object();
  
  void doSomething();
};

//Source
Object::Object() {
  /* ... */
}

void Object::doSomething() {
  /* ... */
}
```

### New Way

```c++
// Header
class Object {
public:
  Object();
  
  void doSomething();
};

// Source
Object::{
  Object() {
    /* ... */
  }
  
  void doSomething() {
    /* ... */
  }
}
```

### With templates

```c++
template<typename T>
class Object {
public:
  Object();
  
  void doSomething();
};

template<typename T>
Object<T>::{
  Object() {
    /* ... */
  }
  
  void doSomething() {
    /* ... */
  }
}
```

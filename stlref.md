# Vector
#### Initialization
```
vector<int> v; // empty vector
vector<int> v(69); // empty vector of size 69
vector<int> v(69, 3); // vector of size 69 filled with 3's
vector<int> v = {1, 2, 3, 4, 5, 6}; // vector with pre-defined elements list
vector<int> v(w.begin(), w.end()) // vector with elements from another vector
```
#### Access
```
v.front() // return the first element
v.back() // return the last element
v.at(i) // return the ith element if present
```
#### Iterators
```
v.begin() // return iterator to the beginning
v.end() // return iterator to the end
v.rbegin() // return reverse iterator to the beginning
v.rend() // return reverse iterator to the end
```
#### Capacity
```
v.size() // return the number of elements
v.empty() // return true if empty false otherwise
v.max_size() // return maximum possible number of elements
```
#### Modifiers
```
v.clear() // clear the contents
v.insert(it, x) // insert x before position it
v.push_back(x) // add x to the back
v.pop_back() // remove the last element
v.erase(it) // remove element at position it
v.erase(it1, it2) // remove elements between it1 and it2
v.resize(n) // resize to store n elements
v.resize(n, k) // resize to store n elements initialized with value k
```
#### Iteration
```
for (int i=0; i<v.size(); i++) { cout << v[i] << endl; }
for (auto it=v.begin(); it!=v.end(); ++it) { cout << *it << endl; }
for (auto x : v) { cout << x << endl; }
```

# Pair
#### Initialization
```
pair<int, int> p; // empty pair
pair<int, int> p(6, 9); // pair with first element 6 and second element 9
pair<int, int> p = make_pair(6, 9); // pair with first element 6 and second element 9
pair<int, int> p; p.first = 6; p.second = 9; // pair with first element 6 and second element 9
```
#### Access
```
p.first // return the first element
p.second // return the second element
```
#### Operators
```
p == q // return true if both elements are equal
p != q // return true if any element is different
p (>)(<)(>=)(<=) q // compare using only the first element
```

# Set
#### Initialization
```
set<int> s; // empty set
set<int> s = {1, 2, 3, 4, 5, 6}; // set with pre-defined elements list
set<int> s(t.begin(), t.end()) // set with elements from another set
```
#### Iterators
```
s.begin() // return iterator to the beginning
s.end() // return iterator to the end
s.rbegin() // return reverse iterator to the beginning
s.rend() // return reverse iterator to the end
```
#### Capacity
```
s.size() // return the number of elements
s.empty() // return true if empty false otherwise
s.max_size() // return maximum possible number of elements
```
#### Modifiers
```
s.clear() // clear the contents
s.insert(x) // insert element x if not present
s.erase(x) // remove element x if present
s.erase(it) // remove element at position it
s.erase(it1, it2) //remove elements between it1 and it2
```
#### Lookup
```
s.find(x) // return iterator if present s.end() otherwise
s.count(x) // return 1 if present 0 otherwise
```
#### Iteration
```
for (auto it=s.begin(); it!=s.end(); ++it) { cout << *it << endl; }
for (auto x : s) { cout << x << endl; }
```

# Map
#### Initialization
```
map<int, int> m; // empty map
map<int, int> m(n.begin(), n.end()) // map with elements from another map
```
#### Iterators
```
m.begin() // return iterator to the beginning
m.end() // return iterator to the end
m.rbegin() // return reverse iterator to the beginning
m.rend() // return reverse iterator to the end
```
#### Capacity
```
m.size() // return the number of elements
m.empty() // return true if empty false otherwise
m.max_size() // return maximum possible number of elements
```
#### Modifiers
```
m.clear() // clear the contents
m.insert(x) // insert element x with key x.first and value x.second if key not present
m.erase(x) // remove element with key x if present
m.erase(it) // remove element at position it
m.erase(it1, it2) //remove elements between it1 and it2
```
#### Lookup
```
m.find(x) // return iterator if present m.end() otherwise
m.count(x) // return 1 if present 0 otherwise
```
#### Iteration
```
for (auto it=m.begin(); it!=m.end(); ++it) { cout << (*it).first << " " << (*it).second << endl; }
for (auto x : s) { cout << x.first << " " << x.second << endl; }
```

# Stack
#### Initialization
```
stack<int> s; // empty stack
```
#### Access
```
s.top() // return reference to the top element
```
#### Capacity
```
s.size() // return the number of elements
s.empty() // return true if empty false otherwise
```
#### Modifiers
```
s.push(x) // insert element x at the top
s.pop() // remove the top element
```

# Queue
#### Initialization
```
queue<int> q; // empty queue
```
#### Access
```
q.front() // return reference to the first element
q.back() // return reference to the last element
```
#### Capacity
```
q.size() // return the number of elements
q.empty() // return true if empty false otherwise
```
#### Modifiers
```
q.push(x) // insert element x at the back
q.pop() // remove the first element
```

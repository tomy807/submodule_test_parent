## 1 add submodule

```
$git submodule add https://github.com/tomy807/submodule_test_child.git
```

.gitmodules

```
[submodule "submodule_test_child"]
	
    path = submodule_test_child

	url = https://github.com/tomy807/submodule_test_child.git
```
## 2 clone git with submodule
```
if git clone https://github.com/tomy807/submodule_test_parent.git
```
submodule을 포함하는 git을 클론 할시 submodule은 함께 클론 되지 않고 빈 폴더만 클론 된다.
```
git submodule update --init
```
하면 submodule도 불러올수 있다.

## 3 update submodules at once
한번에 모든 서브모듈을 update함.

```
git submodule update --remote
```

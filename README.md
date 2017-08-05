# TaduSdk


```php
  Kint::dump(TaduLib::getInstance()->getBookCount());
        Kint::dump(TaduLib::getInstance()->getBookList(1));
        Kint::dump(TaduLib::getInstance()->getBookDetail(234));
        exit();
        Kint::dump(
            TaduLib::getInstance()->addBook(
                [
                    'cpid' => '234',
                    'coverimage' => 'https://www.test.com/aaa.jpg',
                    'bookname' => '我的金主是情痴',
                    'authorname' => '聊了了',
                    'intro' => 'biyu biyu dskfjlskdf',
                    'classid' => 104,
                    'serial' => 1,
                    'isvip' => 1,
                    'url' => 'https://m.ffffff.cc/?novelId=190009&page=SharePage/TFNovelDetailMain.js'
                ]));
        Kint::dump(
            TaduLib::getInstance()->updateBook(
                [
                    'cpid' => '234',
                    'intro' => 'biyu biyu dskfjlskdf2',
                    'classid' => 105,
                    'serial' => 0
                ]));
        Kint::dump(
            TaduLib::getInstance()->updateCover(
                [
                    'cpid' => '234',
                    'coverimage' => 'new image url'
                ]));
        Kint::dump(TaduLib::getInstance()->deleteBook([
            'cpid' => '23411'
        ]));
        Kint::dump(TaduLib::getInstance()->getUpdateInfo([
            'cpid' => '234'
        ]));
        Kint::dump(TaduLib::getInstance()->getChapterList([
            'cpid' => '234'
        ]));
        Kint::dump(
            TaduLib::getInstance()->getChapterDetail(
                [
                    'cpid' => '234',
                    'chapterid' => 111
                ]));
        Kint::dump(
            TaduLib::getInstance()->addChapter(
                [
                    'cpid' => '234',
                    'bookid' => 2340324,
                    'title' => 'sdfsd',
                    'content' => 'diaosdkfjsdlkf',
                    'chapternum' => 1,
                    'isvip' => 1, #是否收费 1收费0免费
                    'chapterid' => 1112,
                    'updatemode' => 1 # 状态：1为新增章节 2为修改章节
                ]));
        Kint::dump(
            TaduLib::getInstance()->deletePart(
                [
                    'cpid' => '234232',
                    'chapterid' => 111112
                ]));
```

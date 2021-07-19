
func diziBirlestir (dizi1 : [Int], dizi2: [Int]) {

    var esitlenenDeger : Int
    var arrayResult = [Int]()

    if dizi1.count > dizi2.count {
        esitlenenDeger = dizi2.count
        arrayResult = zip(dizi1,dizi2).map(+)

        for i in esitlenenDeger...dizi1.count-1 {
            arrayResult.append(dizi1[i])
        }
    }else{
        esitlenenDeger = dizi1.count
        arrayResult = zip(dizi1,dizi2).map(+)

        for i in esitlenenDeger...dizi2.count-1 {
            arrayResult.append(dizi2[i])
        }
    }
    print(arrayResult)
}

diziBirlestir(dizi1: [1,1,1,1,1,1,1], dizi2: [1,1,1,1,1,1,1,1,1,1,1,1,1])



pesoPino :: (Ord a, Num a) => a -> a
pesoPino altura 
    |altura <= 300 = altura*3
    |otherwise = (300*3) + ((altura-300)*2)

espesoUtil :: (Ord b,Num b) => b -> Bool
espesoUtil peso 
    | peso>= 400 && peso<=1000 = True
    | otherwise = False

sirvePino :: (Ord a,Num a) => a -> String
sirvePino x 
    |espesoUtil (pesoPino x) = "Un pino de este peso le sirve a la fabrica"
    |otherwise = "No le sirve este peso a la fabrica "





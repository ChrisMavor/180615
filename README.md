# 180615
working on normilzation vector
def vectorSubtract()

def orthogDecomp(v,q):
  r= v
  for i in range(len(q)):
    tempScalar = dot(q[i],v)
    tempVector = scalarVectorMulti(tempScalar, q[i])
    r = vectorSubtract(r,tempVector)

def orthonormDecomp(v,q):
  r = orthogDecomp(v,q)
  status = True
  for i in range(len(r)):
    if r[i] !=0:
      status = False
  if (status == False):
    return normalize(r)
  else:
    return range


def normalize(vector1):


q = [[-4/6,1],[1,2/3]]
v = [1,1]

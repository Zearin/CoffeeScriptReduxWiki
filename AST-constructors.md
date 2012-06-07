* Block :: [Statement] -> Block
* Continue :: Continue
* Break :: Break
* Throw :: Exprs -> Throw
* Return :: Exprs -> Return
* Int :: float -> Int
* Float :: float -> Float
* String :: string -> String
* Undefined :: Undefined
* Null :: Null
* Bool :: bool -> Bool
* UnaryPlusOp :: Exprs -> UnaryPlusOp
* UnaryNegateOp :: Exprs -> UnaryNegateOp
* NotOp :: Exprs -> NotOp
* BitNotOp :: Exprs -> BitNotOp
* UnaryExistsOp :: Exprs -> UnaryExistsOp
* DoOp :: Exprs -> DoOp
* NewOp :: Exprs -> NewOp
* TypeofOp :: Exprs -> TypeofOp
* IncrementOp :: Exprs -> IncrementOp
* DecrementOp :: Exprs -> DecrementOp
* PostIncrementOp :: Exprs -> PostIncrementOp
* PostDecrementOp :: Exprs -> PostDecrementOp
* InclusiveSlice :: Exprs -> Exprs -> Exprs -> InclusiveSlice
* ExclusiveSlice :: Exprs -> Exprs -> Exprs -> ExclusiveSlice
* UnboundedLeftSlice :: Exprs -> Exprs -> UnboundedLeftSlice
* UnboundedRightSlice :: Exprs -> Exprs -> UnboundedRightSlice
* ShallowCopyArray :: Exprs -> ShallowCopyArray
-- a tree of ConcatOp represents interpolation
* ConcatOp :: Exprs -> Exprs -> ConcatOp
* AndOp :: Exprs -> Exprs -> AndOp
* OrOp :: Exprs -> Exprs -> OrOp
* BitAndOp :: Exprs -> Exprs -> BitAndOp
* BitOrOp :: Exprs -> Exprs -> BitOrOp
* BitXorOp :: Exprs -> Exprs -> BitXorOp
* LeftShiftOp :: Exprs -> Exprs -> LeftShiftOp
* SignedRightShiftOp :: Exprs -> Exprs -> SignedRightShiftOp
* UnsignedRightShiftOp :: Exprs -> Exprs -> UnsignedRightShiftOp
* AddOp :: Exprs -> Exprs -> AddOp
* SubtractOp :: Exprs -> Exprs -> SubtractOp
* MultiplyOp :: Exprs -> Exprs -> MultiplyOp
* DivideOp :: Exprs -> Exprs -> DivideOp
* RemOp :: Exprs -> Exprs -> RemOp
* ExistsOp :: Exprs -> Exprs -> ExistsOp
* LTOp :: Exprs -> Exprs -> LTOp
* LTEOp :: Exprs -> Exprs -> LTEOp
* GTOp :: Exprs -> Exprs -> GTOp
* GTEOp :: Exprs -> Exprs -> GTEOp
* EQOp :: Exprs -> Exprs -> EQOp
* NEQOp :: Exprs -> Exprs -> NEQOp
* InOp :: Exprs -> Exprs -> InOp
* OfOp :: Exprs -> Exprs -> OfOp
* InstanceofOp :: Exprs -> Exprs -> InstanceofOp
* SeqOp :: Exprs -> Exprs -> SeqOp
* ExtendsOp :: Exprs -> Exprs -> ExtendsOp
* MemberAccessOp :: Exprs -> MemberNames -> MemberAccessOp
* SoakedMemberAccessOp :: Exprs -> MemberNames -> SoakedMemberAccessOp
* DynamicMemberAccessOp :: Exprs -> Exprs -> DynamicMemberAccessOp
* SoakedDynamicMemberAccessOp :: Exprs -> Exprs -> SoakedDynamicMemberAccessOp
* ProtoMemberAccessOp :: Exprs -> MemberNames -> ProtoMemberAccessOp
* DynamicProtoMemberAccessOp :: Exprs -> Exprs -> DynamicProtoMemberAccessOp
-- we don't support these, but we should
* SoakedProtoMemberAccessOp :: Exprs -> MemberNames -> SoakedProtoMemberAccessOp
* SoakedDynamicProtoMemberAccessOp :: Exprs -> Exprs -> SoakedDynamicProtoMemberAccessOp
* AssignOp :: Assignables -> Exprs -> AssignOp
* ExistsAssignOp :: Assignables -> Exprs -> ExistsAssignOp
* Splice :: Slices -> Exprs -> Splice
* ClassProtoAssignOp :: MemberNames -> Exprs -> ClassProtoAssignOp
* CompoundAssignAddOp :: Assignables -> Exprs -> CompoundAssignAddOp
* CompoundAssignSubtractOp :: Assignables -> Exprs -> CompoundAssignSubtractOp
* CompoundAssignMultiplyOp :: Assignables -> Exprs -> CompoundAssignMultiplyOp
* CompoundAssignDivideOp :: Assignables -> Exprs -> CompoundAssignDivideOp
* CompoundAssignRemOp :: Assignables -> Exprs -> CompoundAssignRemOp
* CompoundAssignBitAndOp :: Assignables -> Exprs -> CompoundAssignBitAndOp
* CompoundAssignBitOrOp :: Assignables -> Exprs -> CompoundAssignBitOrOp
* CompoundAssignBitXorOp :: Assignables -> Exprs -> CompoundAssignBitXorOp
* CompoundAssignAndOp :: Assignables -> Exprs -> CompoundAssignAndOp
* CompoundAssignOrOp :: Assignables -> Exprs -> CompoundAssignOrOp
* FunctionApplication :: Exprs -> [Arguments] -> FunctionApplication
* SoakedFunctionApplication :: Exprs -> [Arguments] -> SoakedFunctionApplication
* Function :: [Parameters] -> Block -> Function
* BoundFunction :: [Parameters] -> Block -> BoundFunction
* Conditional :: Exprs -> Block -> Block -> Conditional
* While :: Exprs -> Block -> While
* InclusiveRange :: Exprs -> Exprs -> InclusiveRange
* ExclusiveRange :: Exprs -> Exprs -> ExclusiveRange
* Switch :: Exprs -> [(Exprs, Block)] -> Block -> Switch
* Regexp :: string -> Regexp
* Super :: [Arguments] -> Super
* ArrayInitialiser :: [Exprs] -> ArrayInitialiser
* ObjectInitialiser :: [(ObjectInitialiserKeys, Exprs)] -> ObjectInitialiser
* Class :: Maybe Assignable -> Maybe Exprs -> [Exprs] -> Class
* Try :: Block -> Maybe Assignable -> Maybe Block -> Maybe Block -> Try
* JavaScript :: string -> JavaScript
* ForIn :: bool -> Assignable -> Maybe Assignable -> Exprs -> Exprs -> Block -> ForIn
* ForOf :: bool -> Assignable -> Maybe Assignable -> Exprs -> Exprs -> Block -> ForOf
* Splat :: Exprs -> Splat


@ Statements
  * Continue
  * Break
  * Throw
  * Return
  * Exprs

@ Exprs
  * Numbers
  * String
  * Undefined
  * Null
  * Bool
  * ContextMember
  * UnaryOps
  * Slices
  * BinOps
  * FunctionApplication
  * SoakedFunctionApplication
  * Function
  * BoundFunction
  * Conditional
  * While
  * InclusiveRange
  * ExclusiveRange
  * Switch
  * Regexp
  * Super
  * ArrayInitialiser
  * ObjectInitialiser
  * Class
  * Try
  * JavaScript
  * ForIn
  * ForOf

@ Numbers
  * Int
  * Float

@ UnaryOps
  * UnaryPlusOp
  * UnaryNegateOp
  * NotOp
  * BitNotOp
  * UnaryExistsOp
  * DoOp
  * NewOp
  * TypeofOp
  * IncrementOp
  * DecrementOp
  * PostIncrementOp
  * PostDecrementOp

@ Slices
  * InclusiveSlice
  * ExclusiveSlice
  * UnboundedLeftSlice
  * UnboundedRightSlice

@ BinOps
  * ConcatOp
  * BoolOps
  * BitOps
  * MathsOps
  * ExistsOp
  * ComparisonOps
  * InOp
  * OfOp
  * InstanceofOp
  * SeqOp
  * ExtendsOp
  * MemberAccessOps
  * AssignOps

@ BoolOps
  * AndOp
  * OrOp

@ BitOps
  * BitAndOp
  * BitOrOp
  * BitXorOp
  * LeftShiftOp
  * SignedRightShiftOp
  * UnsignedRightShiftOp

@ MathsOps
  * AddOp
  * SubtractOp
  * MultiplyOp
  * DivideOp
  * RemOp

@ ComparisonOps
  * LTOp
  * LTEOp
  * GTOp
  * GTEOp
  * EQOp
  * NEQOp

@ MemberAccessOps
  * MemberAccessOp
  * SoakedMemberAccessOp
  * DynamicMemberAccessOp
  * SoakedDynamicMemberAccessOp
  * ProtoMemberAccessOp
  * DynamicProtoMemberAccessOp
  * SoakedProtoMemberAccessOp
  * SoakedDynamicProtoMemberAccessOp

@ AssignOps
  * AssignOp
  * ExistsAssignOp
  * Splice
  * ClassProtoAssignOp
  * CompoundAssignOps

@ CompoundAssignOps
  * CompoundAssignAddOp
  * CompoundAssignSubtractOp
  * CompoundAssignMultiplyOp
  * CompoundAssignDivideOp
  * CompoundAssignRemOp
  * CompoundAssignBitAndOp
  * CompoundAssignBitOrOp
  * CompoundAssignBitXorOp
  * CompoundAssignAndOp
  * CompoundAssignOrOp

@ ObjectInitialiserKeys
  * IdentifierName
  * String
  * Numbers

@ Arguments
  * Exprs
  * Splat

@ Parameters
  * Assignables
  * AssignOp
  * Splat

@ Assignables
  * IdentifierName
  * MemberAccessOps
  * PositionalDestructuring # TODO
  * NamedDestructuring # TODO

@ MemberNames
  * IdentifierName